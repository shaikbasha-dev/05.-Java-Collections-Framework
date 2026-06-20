17 - Collections Algorithms in Java

1. What are Collections Algorithms?
Collections algorithms are helper methods provided by the Collections class.
They help perform common operations on lists and collections.

2. Important Methods in Collections Class
- sort(List<T>) -> sorts a list
- reverse(List<T>) -> reverses the list
- shuffle(List<T>) -> randomly rearranges elements
- binarySearch(List<T>, key) -> searches a sorted list
- max(Collection<T>) -> returns largest element
- min(Collection<T>) -> returns smallest element
- fill(List<T>, value) -> replaces all elements
- copy(List<T>, List<T>) -> copies values from one list to another

3. Example: Sorting
import java.util.*;

public class CollectionsExample {
    public static void main(String[] args) {
        List<Integer> nums = new ArrayList<>();
        nums.add(30);
        nums.add(10);
        nums.add(20);

        Collections.sort(nums);
        System.out.println(nums); // [10, 20, 30]
    }
}

4. Example: Reverse
Collections.reverse(nums);
System.out.println(nums);

5. Example: Binary Search
Collections.binarySearch(nums, 20);

6. Important Note
For binarySearch to work correctly, the list must be sorted first.

7. Summary
The Collections class provides useful algorithms that simplify common tasks like sorting, searching, and reversing data.
