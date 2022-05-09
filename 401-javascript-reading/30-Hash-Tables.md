# Hash Tables


**Terminology**

In the case of a hashtable, it is used to determine the index of the array. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.


![hashTables](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg/1200px-Hash_table_3_1_1_0_1_0_0_SP.svg.png)


**Example**

Let’s say we have data of Seattle neighborhood names and their corresponding zip codes. Now, we want to be able to search through the data to look up a neighborhood and obtain it’s zip code. We could do this using a for loop that looks through each piece of data one by one until it finds the neighborhood name, then returns the zip code there. This would be an O read operation because it requires searching through each piece of data to find the one piece we want.

The reason why searching for a piece of data in a collection is O isn’t because the array is slow, it’s just that we have to look through all N things in the collection. Instead of adding elements to an array from beginning to end, a hash map uses a «hash function» to place each item at a precise index location, based off it’s key.


> Basically, a hash code turns a key into an integer. Hash codes should never have randomness to them.


 Collisions are solved by changing the initial state of the buckets. Each index in the array is called a «bucket» because it can store multiple key/value pairs. Since different keys can lead to the same bucket it’s important to store the entire key/value pair in the bucket, not just the value.


**Hash function**

A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table.


**Hash table**

It uses a hash function to compute an index into an array in which an element will be inserted or searched. Let us consider string S. You are required to count the frequency of all the characters in this string. The simplest way to do this is to iterate over all the possible characters and count their frequency one by one. The time complexity of this approach is O where N is the size of the string and there are 26 possible characters.

Take an array frequency of size 26 and hash the 26 characters with indices of the array by using the hash function.


**Separate chaining**

The cost of a lookup is that of scanning the entries of the selected linked list for the required key. For this reason, chained hash tables remain effective even when the number of table entries is much higher than the number of slots. For separate chaining, the worst-case scenario is when all the entries are inserted into the same linked list. The lookup procedure may have to scan all its entries, so the worst-case cost is proportional to the number of entries in the table.


**Alternatives to all-at-once rehashing**

Some hash table implementations, notably in real-time systems, cannot pay the price of enlarging the hash table all at once, because it may interrupt time-critical operations. The process of rehashing a bucket's items in accordance with the new hash function is termed as cleaning, which is implemented through command pattern by encapsulating the operations such as.



[Home](../README.md)