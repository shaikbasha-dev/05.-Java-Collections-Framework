11 - LinkedHashMap in Java

1. What is LinkedHashMap?
LinkedHashMap is a class in Java that implements the Map interface.
It is similar to HashMap, but it preserves the insertion order of keys.

2. Why use LinkedHashMap?
LinkedHashMap is useful when you need to:
- store key-value pairs
- keep the order in which keys were inserted
- iterate in the same order as insertion

3. Important Features
- stores key-value pairs
- preserves insertion order
- allows one null key and multiple null values
- does not allow duplicate keys

4. Syntax
import java.util.LinkedHashMap;

LinkedHashMap<String, Integer> map = new LinkedHashMap<>();

5. Common Methods
- put(key, value) -> adds or updates the value
- get(key) -> retrieves value by key
- remove(key) -> removes entry
- containsKey(key) -> checks if key exists
- containsValue(value) -> checks if value exists
- size() -> returns number of entries

6. Example Program
import java.util.LinkedHashMap;

public class LinkedHashMapExample {
    public static void main(String[] args) {
        LinkedHashMap<String, Integer> marks = new LinkedHashMap<>();

        marks.put("Alice", 90);
        marks.put("Bob", 85);
        marks.put("Charlie", 95);

        System.out.println(marks); // {Alice=90, Bob=85, Charlie=95}
        for (String key : marks.keySet()) {
            System.out.println(key + " -> " + marks.get(key));
        }
    }
}

7. LinkedHashMap vs HashMap
- HashMap is faster for some operations
- LinkedHashMap preserves insertion order
- HashMap does not guarantee order

8. Summary
LinkedHashMap is useful when you need both fast key-based access and predictable iteration order.
