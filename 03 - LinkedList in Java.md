03 - LinkedList in Java

1. What is LinkedList?
LinkedList is a class in Java that implements the List and Deque interfaces.
It stores elements using nodes, where each node points to the next node.

2. Why use LinkedList?
LinkedList is useful when you need to:
- insert or remove elements frequently
- work with data in front/back positions
- use stack or queue-like behavior

3. Important Features
- stores elements as nodes
- allows duplicate values
- maintains insertion order
- faster insertions/deletions in middle compared to ArrayList
- slower random access compared to ArrayList

4. Syntax
import java.util.LinkedList;

LinkedList<String> names = new LinkedList<>();

5. Common Methods
- add(value) -> adds at end
- addFirst(value) -> adds at beginning
- addLast(value) -> adds at end
- removeFirst() -> removes first element
- removeLast() -> removes last element
- getFirst() -> gets first element
- getLast() -> gets last element
- get(index) -> gets element at position
- remove(index) -> removes at position

6. Example Program
import java.util.LinkedList;

public class LinkedListExample {
    public static void main(String[] args) {
        LinkedList<String> fruits = new LinkedList<>();

        fruits.add("Apple");
        fruits.add("Banana");
        fruits.addFirst("Mango");

        System.out.println(fruits); // [Mango, Apple, Banana]
        System.out.println(fruits.get(1)); // Apple

        fruits.removeLast();
        System.out.println(fruits); // [Mango, Apple]
    }
}

7. LinkedList vs ArrayList
- ArrayList uses dynamic array
- LinkedList uses nodes
- ArrayList is better for fast access by index
- LinkedList is better for frequent insertions/removals

8. Summary
LinkedList is a good choice when your program needs frequent changes at the beginning or middle of the list.
