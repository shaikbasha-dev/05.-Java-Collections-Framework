08 - TreeSet in Java

1. What is TreeSet?
TreeSet is a class in Java that implements the SortedSet interface.
It stores unique elements in sorted order.

2. Why use TreeSet?
TreeSet is useful when you need to:
- store unique values
- keep elements in sorted order automatically
- retrieve elements in natural or custom sorted order

3. Important Features
- no duplicate elements allowed
- elements are stored in sorted order
- does not preserve insertion order
- works with comparable or comparator-based sorting

4. Syntax
import java.util.TreeSet;

TreeSet<Integer> numbers = new TreeSet<>();

5. Common Methods
- add(value) -> adds element
- remove(value) -> removes element
- contains(value) -> checks if present
- first() -> gets first (smallest) element
- last() -> gets last (largest) element
- size() -> returns number of elements
- clear() -> removes all elements

6. Example Program
import java.util.TreeSet;

public class TreeSetExample {
    public static void main(String[] args) {
        TreeSet<Integer> numbers = new TreeSet<>();

        numbers.add(50);
        numbers.add(10);
        numbers.add(30);
        numbers.add(10); // duplicate, ignored

        System.out.println(numbers); // [10, 30, 50]
        System.out.println(numbers.first()); // 10
        System.out.println(numbers.last()); // 50
    }
}

7. TreeSet vs HashSet
- HashSet is faster for general operations
- TreeSet keeps elements sorted
- TreeSet is slightly slower due to sorting logic

8. Summary
TreeSet is ideal when you need a set that always keeps values in sorted order.
