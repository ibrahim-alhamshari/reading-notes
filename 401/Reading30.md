# Hashtable

- It is similar to HashMap, but is synchronized.
- Hashtable stores **key/value** pair in hash table.
- In Hashtable we specify an object that is used as a key, and the - value we want to associate to that key. The key is then hashed, and the resulting hash code is used as the index at which the value is stored within the table.

![Hash table](https://howtodoinjava.com/wp-content/uploads/2018/10/hashtable.gif)

* **Terminology:**
    - Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.

    - Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

    - Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

- **methods that we can implement:**
1. Add()
- We use it to add a new key/value pair to a hashtable.
2. find() 
-  Takes a key, gets the Hash, and goes to the index location specified.
3. Contains()
-  It accepts a key, and returns a bool on if that key exists inside the hashtable or not.
4. GetHash()
- It accepts a key as a string, conducts the hash, and then returns the index of the array where the key/value should be placed.

### Ressources
- [Hashtable](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- [video_HashTable](https://www.youtube.com/watch?v=MfhjkfocRR0)
- [basics-of-hash-tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- [Hash_Table](https://en.wikipedia.org/wiki/Hash_table)