18 - Collections vs Collection in Java

1. Collection
Collection is an interface in Java.
It is the root interface for all collection classes like List, Set, and Queue.

2. Collections
Collections is a utility class.
It contains static methods for performing common operations on collections, such as sorting, searching, and reversing.

3. Main Difference
- Collection -> interface for data structures
- Collections -> helper class with utility methods

4. Example
import java.util.*;

public class CollectionVsCollections {
    public static void main(String[] args) {
        List<String> names = new ArrayList<>();
        names.add("Java");
        names.add("Python");

        Collections.sort(names); // using Collections class
        System.out.println(names);
    }
}

5. Summary
Collection is a type of data structure interface, while Collections is a class with useful algorithms for working with those structures.
