14 - Wrapper Classes in Java

1. What are Wrapper Classes?
Wrapper classes are classes that wrap primitive data types into objects.
For example, int is wrapped by Integer, char by Character, and boolean by Boolean.

2. Why do we need Wrapper Classes?
Wrapper classes are needed because:
- collections store objects, not primitives
- some APIs require objects instead of primitive values
- wrapper classes provide useful methods

3. Common Wrapper Classes
- Integer for int
- Float for float
- Double for double
- Long for long
- Character for char
- Boolean for boolean
- Short for short
- Byte for byte

4. Autoboxing and Unboxing
Autoboxing: converting primitive to wrapper object automatically.
Unboxing: converting wrapper object back to primitive automatically.

5. Example Program
import java.util.ArrayList;

public class WrapperExample {
    public static void main(String[] args) {
        ArrayList<Integer> numbers = new ArrayList<>();
        numbers.add(10);      // autoboxing
        numbers.add(20);

        int a = numbers.get(0); // unboxing
        System.out.println(a);  // 10
    }
}

6. Important Methods
- parseInt("123") -> converts string to int
- toString(value) -> converts primitive to string
- valueOf(...) -> returns wrapper object

7. Summary
Wrapper classes allow primitives to be used in object-oriented contexts, especially in collections and APIs.
