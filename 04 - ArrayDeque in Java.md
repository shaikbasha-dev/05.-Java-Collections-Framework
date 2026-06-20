04 - ArrayDeque in Java

1. What is ArrayDeque?
ArrayDeque is a class in Java that implements the Deque interface.
It represents a resizable array-based deque (double-ended queue).

2. Why use ArrayDeque?
ArrayDeque is useful when you need to:
- add/remove elements from both ends
- use queue or stack behavior
- improve performance compared to LinkedList for many operations

3. Important Features
- supports insertion and deletion from both front and back
- does not allow null elements
- faster than LinkedList for most deque operations
- not synchronized by default

4. Syntax
import java.util.ArrayDeque;

ArrayDeque<String> deque = new ArrayDeque<>();

5. Common Methods
- addFirst(value) -> adds at front
- addLast(value) -> adds at end
- removeFirst() -> removes first element
- removeLast() -> removes last element
- getFirst() -> gets first element
- getLast() -> gets last element
- offer(value) -> adds at end
- poll() -> removes and returns first element
- peek() -> gets first element without removing

6. Example Program
import java.util.ArrayDeque;

public class ArrayDequeExample {
    public static void main(String[] args) {
        ArrayDeque<Integer> deque = new ArrayDeque<>();

        deque.addFirst(10);
        deque.addLast(20);
        deque.addLast(30);

        System.out.println(deque); // [10, 20, 30]
        System.out.println(deque.peek()); // 10

        deque.removeFirst();
        System.out.println(deque); // [20, 30]
    }
}

7. ArrayDeque vs LinkedList
- ArrayDeque is array-based and faster for deque operations
- LinkedList is node-based and supports null values
- ArrayDeque is better for queue/stack-style usage

8. Summary
ArrayDeque is a very efficient choice when you need to work with elements from both ends of a collection.
