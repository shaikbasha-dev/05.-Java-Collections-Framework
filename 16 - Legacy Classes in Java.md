16 - Legacy Classes in Java

1. What are Legacy Classes?
Legacy classes are older collection classes that were part of Java before the Java Collections Framework was fully developed.
They are still available, but modern code usually prefers newer classes.

2. Common Legacy Classes
- Vector
- Stack
- Hashtable
- Dictionary

3. Vector
Vector is a synchronized dynamic array.
It is similar to ArrayList, but it is thread-safe.

4. Stack
Stack is a subclass of Vector.
It follows LIFO (Last In, First Out) order.

5. Hashtable
Hashtable is a synchronized map implementation.
It stores key-value pairs and does not allow null keys or null values.

6. Dictionary
Dictionary is an abstract class that represents key-value storage.
It is an older base class for Hashtable.

7. Why are Legacy Classes Less Preferred?
- they are synchronized unnecessarily in many cases
- they are older APIs
- modern alternatives like ArrayList, HashMap, and Deque are more flexible and efficient

8. Example Program
import java.util.*;

public class LegacyExample {
    public static void main(String[] args) {
        Vector<String> vector = new Vector<>();
        vector.add("Java");
        vector.add("Python");

        System.out.println(vector);

        Hashtable<String, Integer> table = new Hashtable<>();
        table.put("A", 1);
        table.put("B", 2);

        System.out.println(table);
    }
}

9. Summary
Legacy classes are important for understanding Java history, but modern applications usually use the newer collection classes.
