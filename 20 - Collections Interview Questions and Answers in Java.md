20 - Collections Interview Questions and Answers in Java

1. What is the Java Collections Framework?
Answer:
The Java Collections Framework is a set of classes and interfaces in java.util that helps store and manipulate groups of objects efficiently.

2. What is the difference between Collection and Collections?
Answer:
Collection is an interface for the collection hierarchy, while Collections is a utility class that contains static methods like sort(), reverse(), and binarySearch().

3. What is the difference between List, Set, and Map?
Answer:
List stores ordered elements and allows duplicates.
Set stores unique elements and does not allow duplicates.
Map stores key-value pairs.

4. What is the difference between ArrayList and LinkedList?
Answer:
ArrayList uses a dynamic array and is better for fast random access.
LinkedList uses nodes and is better for frequent insertions and deletions.

5. What is the difference between ArrayList and Vector?
Answer:
ArrayList is not synchronized and is faster for most single-threaded use.
Vector is synchronized and thread-safe.

6. What is the difference between HashSet and TreeSet?
Answer:
HashSet stores elements in no guaranteed order and is faster.
TreeSet stores elements in sorted order.

7. What is the difference between HashMap and TreeMap?
Answer:
HashMap stores data in no guaranteed order and is faster.
TreeMap stores keys in sorted order.

8. What is the difference between HashMap and Hashtable?
Answer:
HashMap is not synchronized and allows null values.
Hashtable is synchronized and does not allow null keys or values.

9. What is the difference between HashSet and LinkedHashSet?
Answer:
HashSet does not maintain insertion order.
LinkedHashSet maintains insertion order.

10. What is the difference between HashMap and LinkedHashMap?
Answer:
HashMap does not guarantee order.
LinkedHashMap preserves insertion order.

11. Why is HashSet not allowed to store duplicate values?
Answer:
HashSet uses the hashCode() and equals() methods to determine uniqueness. If two objects are equal, the second one is ignored.

12. What is the purpose of equals() and hashCode()?
Answer:
equals() checks whether two objects are logically equal.
hashCode() returns a hash value used for efficient storage and lookup in hash-based collections.

13. What is autoboxing and unboxing?
Answer:
Autoboxing converts primitive values into wrapper objects automatically.
Unboxing converts wrapper objects back into primitive values automatically.

14. Why do we need wrapper classes in collections?
Answer:
Collections store objects, so primitive values must be wrapped in classes like Integer, Double, and Boolean.

15. What is PriorityQueue?
Answer:
PriorityQueue is a queue where elements are processed according to their priority, not insertion order.

16. What is the difference between Queue and PriorityQueue?
Answer:
Queue follows FIFO order.
PriorityQueue processes elements based on priority.

17. What is ArrayDeque used for?
Answer:
ArrayDeque is used for implementing a double-ended queue efficiently, especially for insertions and removals from both ends.

18. What is the difference between Iterator and ListIterator?
Answer:
Iterator is used to traverse collections in one direction.
ListIterator is used for lists and allows traversal in both directions.

19. What is the difference between fail-fast and fail-safe iterators?
Answer:
Fail-fast iterators throw ConcurrentModificationException if the collection is modified during iteration.
Fail-safe iterators do not throw exceptions because they work on a copy of the collection.

20. Which collection should you use when you need sorted unique elements?
Answer:
You should use TreeSet if you need sorted unique elements.

21. Which collection should you use when you need key-value pairs with insertion order?
Answer:
You should use LinkedHashMap.

22. Which collection should you use when you need fast lookup by key?
Answer:
You should use HashMap.

23. What is the purpose of Collections.sort()?
Answer:
It sorts the elements of a List in natural order.

24. What is the difference between Comparable and Comparator?
Answer:
Comparable is implemented by the class itself to define natural ordering.
Comparator is separate and used to define custom sorting logic.

25. What is the use of Collections.reverse()?
Answer:
It reverses the order of elements in a List.

26. What is the difference between map.keySet(), map.values(), and map.entrySet()?
Answer:
keySet() returns all keys.
values() returns all values.
entrySet() returns all key-value pairs.

27. What is a synchronized collection?
Answer:
A synchronized collection is thread-safe and can be used safely in multi-threaded programs.

28. What is a mutable and immutable collection?
Answer:
A mutable collection can be changed after creation.
An immutable collection cannot be changed once created.

29. Why is TreeMap slower than HashMap?
Answer:
Because TreeMap keeps elements sorted using red-black tree operations, which take extra time compared to HashMap's hashing.

30. Can you store null values in HashMap?
Answer:
Yes, HashMap allows one null key and multiple null values.
