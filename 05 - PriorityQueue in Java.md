05 - PriorityQueue in Java

1. What is PriorityQueue?
PriorityQueue is a class in Java that implements the Queue interface.
It stores elements in a priority order, so the smallest or highest priority element is processed first.

2. Why use PriorityQueue?
PriorityQueue is useful when you need to:
- process elements based on priority
- efficiently retrieve the highest/lowest priority element
- use a queue with ordering rules

3. Important Features
- does not allow null elements
- does not preserve insertion order
- elements are ordered according to natural ordering or comparator
- is not synchronized by default

4. Syntax
import java.util.PriorityQueue;

PriorityQueue<Integer> pq = new PriorityQueue<>();

5. Common Methods
- add(value) -> inserts an element
- offer(value) -> inserts an element
- poll() -> removes and returns the smallest/highest priority element
- peek() -> gets the head element without removing it
- size() -> returns number of elements
- contains(value) -> checks if value exists

6. Example Program
import java.util.PriorityQueue;

public class PriorityQueueExample {
    public static void main(String[] args) {
        PriorityQueue<Integer> pq = new PriorityQueue<>();

        pq.add(50);
        pq.add(10);
        pq.add(30);

        System.out.println(pq); // may print in heap order
        System.out.println(pq.poll()); // 10
        System.out.println(pq.poll()); // 30
        System.out.println(pq.poll()); // 50
    }
}

7. PriorityQueue vs Queue
- Queue follows FIFO order (first in, first out)
- PriorityQueue orders elements by priority
- Queue is simple order-based processing
- PriorityQueue is priority-based processing

8. Summary
PriorityQueue is used when elements should be processed according to their priority rather than insertion order.
