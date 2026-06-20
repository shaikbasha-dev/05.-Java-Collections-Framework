02 - ArrayList in Java

1. What is ArrayList?
ArrayList is a class in Java that implements the List interface.
It stores elements in a dynamic array and allows duplicates.

2. Why use ArrayList?
ArrayList is used when you need a collection that:
- can grow or shrink in size
- stores multiple values
- allows easy access by index
- supports many built-in methods

3. Important Features
- dynamic size
- maintains insertion order
- allows duplicate values
- elements can be accessed using index
- not synchronized by default

4. Syntax
import java.util.ArrayList;

ArrayList<String> names = new ArrayList<>();

5. Common Methods
- add(value) -> adds an element
- add(index, value) -> adds at a specific position
- get(index) -> gets an element
- set(index, value) -> updates an element
- remove(index) -> removes an element
- size() -> returns number of elements
- contains(value) -> checks if element exists
- clear() -> removes all elements

6. Example Program
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        ArrayList<String> fruits = new ArrayList<>();

        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Mango");

        System.out.println(fruits); // [Apple, Banana, Mango]
        System.out.println(fruits.get(1)); // Banana

        fruits.set(1, "Orange");
        System.out.println(fruits); // [Apple, Orange, Mango]
    }
}

7. Difference between Array and ArrayList
- Array has fixed size
- ArrayList is dynamic
- Array can store primitive types directly
- ArrayList stores objects only

8. Summary
ArrayList is one of the most commonly used collection classes in Java.
It is best when you need a flexible ordered list of elements.
