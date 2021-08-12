# Implementation: Hash Tables

## Define teh following terms:
1. Hash :  hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
<br/>

2. Buckets : A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
<br/>

3. Collisions : A collision is what happens when more than one key gets hashed to the same location of the hashtable.


<br/>
<br/>
<br/>


## Why do we use HashTables?
- Hold unique values(For security).
- Dictionary.
- Library.
<br/>
<br/>
<br/>


## What are HashTables exactly ?
- a data structure that utilize key value pairs. This means every `Node` or `Bucket` has both a key, and a value.
<br/>
<br/>
<br/>


## What is the basic idea of HashTables?
- The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value.
- Basically, a hash code turns a key into an integer.
<br/>
<br/>
<br/>

## What is the time complexity for a lookup in stored Values with HashTables?
- we can do a lookup in an O(1) time complexity.
<br/>
<br/>
<br/>


## The worse possible Hash ...

 > the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.
<br/>
<br/>
<br/>


## What does Hash maps do  to store value?

- accept a key.
- calculate the hash of the key.
- use modulus to convert the hash into an array index.
- store the key with the value by appending both to the end of a linked list.
<br/>
<br/>



## What does Hash maps do  to read value?
- accept a key.
- calculate the hash of the key.
- use modulus to convert the hash into an array index.
- use the array index to access the short LinkedList representing a bucket
- search through the bucket looking for a node with a key/value pair that matches the key you were given.
<br/>
<br/>



## some Internal Methods to use with HashTables:

### Add()

- send the key to the GetHash method.
- Once you determine the index of where it should be placed, go to that index
- Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
- If something does exist, add the new key/value pair to the data structure within that bucket.
<br/>
<br/>

### Find()
- The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.
<br/>
<br/>

### Contains()
- The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.
<br/>
<br/>


### GetHash()
- The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
<br/>
<br/>

## What is a Hash function?
- A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. 

- The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.
<br/>
<br/>

 ## What is Double Hashing?
  - Double hashing is similar to linear probing and the only difference is the interval between successive probes. Here, the interval between probes is computed by using two hash functions.

<br/>
<br/>
<br/>
<br/>

## References:

- [What is a Hashtable?](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html).

- [https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/).