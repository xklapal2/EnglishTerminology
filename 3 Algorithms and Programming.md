## Algorithms and Programming


### Problem-solving example

How to design an efficient search and filter algorithm for products.

- **Solution: TF-IDF (Term Frequency-Inverse Document Frequency) Algorithm**
- **How it fits to our use-case**: The TF-IDF algorithm calculates the relevance of each product to the user’s search query. Here is the process: 
	- The query is broken into tokens (words or phrases)
	- The algorithm computes the frequency of each token in the product's name, parameters, or description **(Term Frequency)**
	- It also calculates the **Inverse Document Frequency**, which reflects how important a token is across the entire product inventory (less common terms are given more weight).
	- By combining the TF and IDF values for each token, the algorithm calculates a score for each product.
	- The products are then ranked based on their relevance score, ensuring the most relevant products appear at the top of the search results.

### Algorithm design

Sorting algorithms for showing products by price or popularity.

- **Solution:** A **Quick Sort** algorithm can be used for efficiently handling large product lists.
- **Example :** In this option **Quick Sort** partitions the list of products based on their prices. The algorithm then recursively sorts the products in requested order.


### Implementation example

Writing a sorting or recommendation algorithm in Python/Java/C# that takes user preferences and displays relevant products.

```
products = REQUEST_FROM_DB 

# Perform TF-IDF search
relevantProducts = tf_idf_search(query, products)

# Simple Quick Sort Algorithm, where sort by can be popularity or price 
def quickSort(relevantProducts, order, sort_by): 
    if len(relevantProducts) <= 1:
        return relevantProducts
    
    pivot = relevantProducts[0]
    pivot_value = pivot[sort_by]
    left = []
    right = []
    
    for product in relevantProducts[1:]:
        product_value = product[sort_by]
        
        if order == 'desc':
            if product_value < pivot_value:
                left.append(product)
            else:
                right.append(product)
        else:
            if product_value > pivot_value:
                left.append(product)
            else:
                right.append(product)
    
    sorted_left = quickSort(left, order, sort_by)
    sorted_right = quickSort(right, order, sort_by)
    
    return sorted_left + [pivot] + sorted_right
```