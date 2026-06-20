09 - Hashing in Java

1. What is Hashing?
Hashing is a technique used to convert data into a fixed-size value called a hash code.
This hash code helps in fast storage and retrieval of data.

2. Purpose of Hashing
Hashing is used to:
- store data efficiently
- search data quickly
- reduce lookup time in collections like HashMap and HashSet

3. Hash Code
A hash code is an integer value generated from an object.
Two equal objects should usually have the same hash code.

4. How Hashing Works
- A key is passed to a hash function.
- The hash function produces an index.
- The index is used to store or find the value.

5. Importance in Collections
Hashing is the base idea behind:
- HashMap
- HashSet
- LinkedHashMap
- LinkedHashSet

6. Example
public class HashExample {
    public static void main(String[] args) {
        String name = "Java";
        System.out.println(name.hashCode());
    }
}

7. Collision
A collision happens when two different keys produce the same hash code.
Java handles collisions using data structures like linked lists or balanced trees.

8. Summary
Hashing is an efficient way to store and retrieve data.
It is one of the main reasons why hash-based collections work so fast.
