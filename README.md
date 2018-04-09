#Implicit ALS notebook

In this notebook we run implicit ALS on a set of data taken from http://www2.informatik.uni-freiburg.de/~cziegler/BX/.The notebook requires that you have downloaded the following files:
1. BX-Book-Ratings.csv
2. BX-Books.csv

From the BX-Book-Ratings.csv file, we wish to extract rows where the 'ratings' are equal to 0, denoting an implicit interaction between the user and the book. This can be done using the following command, run from a bash terminal:
```bash
grep '"0"' BX-Book-Ratings.csv > implicit.csv
```
The desired rows are now held in the file implicit.csv. This will then be ingested by the Implicit ALS notebook. 
