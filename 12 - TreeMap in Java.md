12 - TreeMap in Java

1. What is TreeMap?
TreeMap is a class in Java that implements the Map interface.
It stores key-value pairs in sorted order according to the keys.

2. Why use TreeMap?
TreeMap is useful when you need to:
- store elements in sorted key order
- retrieve the smallest or largest key easily
- use key-based lookup with ordering

3. Important Features
- stores key-value pairs
- keys are sorted automatically
- does not allow duplicate keys
- does not preserve insertion order

4. Syntax
import java.util.TreeMap;

TreeMap<String, Integer> map = new TreeMap<>();

5. Common Methods
- put(key, value) -> inserts or updates value
- get(key) -> retrieves value
- remove(key) -> removes entry
- firstKey() -> gets smallest key
- lastKey() -> gets largest key
- containsKey(key) -> checks if key exists
- size() -> returns number of entries

6. Example Program
import java.util.TreeMap;

public class TreeMapExample {
    public static void main(String[] args) {
        TreeMap<String, Integer> marks = new TreeMap<>();

        marks.put("B", 80);
        marks.put("A", 90);
        marks.put("C", 85);

        System.out.println(marks); // {A=90, B=80, C=85}
        System.out.println(marks.firstKey()); // A
        System.out.println(marks.lastKey()); // C
    }
}

7. TreeMap vs HashMap
- HashMap is faster for general access
- TreeMap keeps keys sorted
- TreeMap is useful when ordering matters

8. Summary
TreeMap is a good choice when you want sorted key-based storage in Java.
