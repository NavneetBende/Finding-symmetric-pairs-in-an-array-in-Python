Symmetric pairs in array in Python
In this page you will find the program to print all symmetric pairs in an array in python programming language. We are given with an array and need to print the all symmetric pairs present in the given array.

symmetric pairs in an array in Python
Explanation :
We are given with pairs, some symmetric pairs are exists in the given set of pairs. The problem statement says that we have to find all symmetric pairs that exist
Example,
Input : arr[5][2] = {{10,20}, {30,40}, {50,60}, {20,10}, {40,30}, {90, 100}, {1, 9}, {100, 90}}
Output : (10,20) (30,40) (90, 100)
Algorithm :
Create a set.
Start iterating over pairs.
Insert the pair in set
Check if(y, x) exist in the set,
If yes, then print that element.
Set in Python
Sets are used to store multiple items in a single variable. Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage.
A Set is an unordered collection data type that is iterable, mutable and has no duplicate elements.
Python's set class represents the mathematical notion of a set.
Related Pages
Finding Maximum scalar product of two vectors in an array

Counting the number of even and odd elements in an array

Find maximum product sub-array in a given array

Finding Arrays are disjoint or not

Determine Array is a subset of another array

Code in Python
Run
# Function to find all pairs that are a mirror of each other
def findPairs(pairs):
 
    # create an empty set of strings
    s = set()
 
    # do for each pair
    for (x, y) in pairs:
 
        # insert the current pair `(x, y)` into the set
        s.add((x, y))
 
        # if mirror pair `(y, x)` is seen before, print the pairs
        if (y, x) in s:
            print((x, y))
 

pairs = [(3, 4), (1, 2), (5, 2), (7, 10), (4, 3), (2, 5)]
findPairs(pairs)
Output
(4, 3)
(2, 5)
