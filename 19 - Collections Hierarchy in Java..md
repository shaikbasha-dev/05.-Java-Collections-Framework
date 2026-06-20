19 - Collections Hierarchy in Java

1. What is the Collections Hierarchy?
The Java Collections Framework is organized into interfaces and classes.
It helps us understand how different collection types are related.

2. Main Root Interface
- Collection
  - List
    - ArrayList
    - LinkedList
    - Vector
  - Set
    - HashSet
    - LinkedHashSet
    - TreeSet
  - Queue
    - PriorityQueue
    - ArrayDeque

3. Map Interface (separate from Collection)
- Map
  - HashMap
  - LinkedHashMap
  - TreeMap
  - Hashtable

4. Important Idea
- Collection is for storing single values
- Map is for storing key-value pairs

5. Example of Hierarchy
Collection
├── List
│   ├── ArrayList
│   ├── LinkedList
│   └── Vector
├── Set
│   ├── HashSet
│   ├── LinkedHashSet
│   └── TreeSet
└── Queue
    ├── PriorityQueue
    └── ArrayDeque

Map
├── HashMap
├── LinkedHashMap
├── TreeMap
└── Hashtable

6. Summary
The collections hierarchy shows how Java organizes data structures.
It helps us select the correct collection type for a problem.
