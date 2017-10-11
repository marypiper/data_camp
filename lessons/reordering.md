

## Reordering data using indices
Often during data wrangling we find it necessary to reorder the elements in a vector or the rows or columns in a data frame. The most basic way to reorder is to use the indices associated with each element in a vector. Indexing `[ ]` can be used to extract values from a dataset as we saw earlier, but we can also use it to rearrange our data values. 

```r
alphabet <- c("C", "F", "G", "A", "D", "E", "B")
```
<img src="../img/alphabet_unordered.png" width="500">

We can extract values in a vector by specifying it's position or index:

```r
alphabet[c(7, 4, 5)] # Extracting values from a vector
alphabet
```

<img src="../img/alphabet_unordered_highlight.png" width="500">

By specifying the element using it's index, we can extract the values from the vector in the order specified.

<img src="../img/alphabet_bad.png" width="210">

Therefore, to reorder values in a vector, we can extract **all of the values** and reorder them by providing the indices in the order we would like output. 

<img src="../img/alphabet_unordered.png" width="500">

Let's reorder the elements to follow the order of the alphabet:

```r
alphabet[c(4, 7, 1, 5, 6, 2, 3)] 
```

<img src="../img/alphabet_ordered.png" width="475">

If we want to save our results, we need to assign to a variable:

```r
ordered_alphabet <- alphabet[c(4, 7, 1, 5, 6, 2, 3)] 
```

