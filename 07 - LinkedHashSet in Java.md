07 - LinkedHashSet in Java

1. What is LinkedHashSet?
LinkedHashSet is a class in Java that implements the Set interface.
It stores unique elements like HashSet, but also maintains insertion order.

2. Why use LinkedHashSet?
LinkedHashSet is useful when you need to:
- store unique values
- preserve the order in which elements were inserted
- iterate in the same order as insertion

3. Important Features
- does not allow duplicate elements
- keeps insertion order
- uses hashing internally for fast access
- allows only one null value

4. Syntax
import java.util.LinkedHashSet;

LinkedHashSet<String> set = new LinkedHashSet<>();

5. Common Methods
- add(value) -> adds element if not already present
- remove(value) -> removes element
- contains(value) -> checks existence
- size() -> returns number of elements
- clear() -> removes all elements
- iterator() -> iterates in insertion order

6. Example Program
import java.util.LinkedHashSet;

public class LinkedHashSetExample {
    public static void main(String[] args) {
        LinkedHashSet<String> fruits = new LinkedHashSet<>();

        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Apple");

        System.out.println(fruits); // [Apple, Banana]
        for (String fruit : fruits) {
            System.out.println(fruit);
        }
    }
}

7. LinkedHashSet vs HashSet
- HashSet does not guarantee order
- LinkedHashSet keeps insertion order
- Both do not allow duplicates

8. Summary
LinkedHashSet is a good choice when you want uniqueness and also want to preserve insertion order.
