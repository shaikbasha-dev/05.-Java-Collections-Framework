13 - Map Views in Java

1. What is a Map View?
A map view is a way to see a Map through another collection interface.
For example, you can view a Map as a set of keys, a collection of values, or a set of entries.

2. Main Map Views
- keySet() -> gives a Set view of the keys
- values() -> gives a Collection view of the values
- entrySet() -> gives a Set view of key-value pairs

3. Why are Map Views Useful?
Map views allow you to:
- iterate over keys or values easily
- perform operations using collection APIs
- access entries as objects

4. Example Program
import java.util.*;

public class MapViewExample {
    public static void main(String[] args) {
        Map<String, Integer> map = new HashMap<>();
        map.put("A", 1);
        map.put("B", 2);
        map.put("C", 3);

        System.out.println(map.keySet());
        System.out.println(map.values());
        System.out.println(map.entrySet());

        for (Map.Entry<String, Integer> entry : map.entrySet()) {
            System.out.println(entry.getKey() + " -> " + entry.getValue());
        }
    }
}

5. Important Notes
- keySet() returns a view, not a copy
- changes in the view reflect in the original map
- entrySet() is commonly used when you need both key and value

6. Summary
Map views help you work with maps using collection-style operations.
They are especially useful when iterating through a map.
