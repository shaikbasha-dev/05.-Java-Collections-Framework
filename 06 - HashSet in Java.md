06 - HashSet in Java

1. What is HashSet?
HashSet is a class in Java that implements the Set interface.
It stores unique elements and does not keep insertion order.

2. Why use HashSet?
HashSet is useful when you need to:
- store unique values only
- perform fast search, insert, and delete operations
- ignore duplicates automatically

3. Important Features
- no duplicate elements allowed
- no guarantee of order
- uses hashing for fast access
- allows only one null value

4. Syntax
import java.util.HashSet;

HashSet<String> set = new HashSet<>();

5. Common Methods
- add(value) -> adds element if not already present
- remove(value) -> removes element
- contains(value) -> checks existence
- size() -> returns number of elements
- clear() -> removes all elements
- iterator() -> iterates through elements

6. Example Program
import java.util.HashSet;

public class HashSetExample {
    public static void main(String[] args) {
        HashSet<String> fruits = new HashSet<>();

        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Apple"); // duplicate, ignored

        System.out.println(fruits); // order may vary
        System.out.println(fruits.contains("Banana")); // true
    }
}

7. HashSet vs ArrayList
- ArrayList allows duplicates and keeps order
- HashSet stores unique elements and does not guarantee order
- ArrayList is better for indexed access
- HashSet is better for uniqueness checks

8. Summary
HashSet is a great choice when you want to store only unique values and perform fast membership checks.
