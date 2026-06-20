01 - Introduction to Collections in Java

1. What is a Collection?
A collection is an object that groups multiple elements into a single unit.
It is used to store, retrieve, manipulate, and iterate data efficiently.

2. Why do we need Collections?
Without collections, we would have to manage arrays manually for every task.
Collections provide built-in methods for:
- adding elements
- removing elements
- searching elements
- sorting elements
- iterating through elements

3. Java Collections Framework (JCF)
The Java Collections Framework is a set of classes and interfaces defined in java.util.
It provides reusable data structures for storing objects.

4. Main Interfaces in Collections Framework
- Collection: root interface for all collections
- List: ordered collection, allows duplicates
- Set: unordered collection, no duplicates
- Queue: holds elements for processing in order
- Map: stores key-value pairs

5. Common Classes
- ArrayList: dynamic array, fast random access
- LinkedList: linked nodes, good for insert/delete
- HashSet: stores unique elements, no order guarantee
- TreeSet: stores unique elements in sorted order
- HashMap: stores key-value pairs, fast lookup
- TreeMap: stores key-value pairs in sorted key order

6. Example
import java.util.*;

public class CollectionExample {
    public static void main(String[] args) {
        List<String> fruits = new ArrayList<>();
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Apple");

        System.out.println(fruits); // [Apple, Banana, Apple]
    }
}

7. Difference between Array and Collection
- Array has fixed size
- Collection is dynamic in size
- Arrays store only homogeneous data (in general)
- Collections can store objects more flexibly

8. Summary
The Collections Framework makes Java programming easier by providing standard data structures.
It helps developers write cleaner, faster, and more maintainable code.
