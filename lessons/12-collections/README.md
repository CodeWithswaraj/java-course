# Lesson 12 — Collections Framework

## Learning objectives
Choose and use common Java collection types.

## List
Ordered collection that permits duplicates.
```java
List<String> names = new ArrayList<>();
names.add("Asha");
names.add("Ravi");
```
Common implementations: `ArrayList`, `LinkedList`.

## Set
Stores unique elements. Common implementations: `HashSet`, `LinkedHashSet`, `TreeSet`.

## Map
Stores key-value pairs.
```java
Map<String, Integer> marks = new HashMap<>();
marks.put("Asha", 92);
System.out.println(marks.get("Asha"));
```
Common implementations: `HashMap`, `LinkedHashMap`, `TreeMap`.

## Queue and Deque
Useful for FIFO and double-ended operations. Common implementations include `ArrayDeque` and priority queues.

## Iteration
```java
for (String name : names) {
    System.out.println(name);
}
```
An `Iterator` is useful when explicit iterator-based traversal or safe removal during iteration is required.

## Choosing a collection
- `ArrayList`: fast indexed access, general-purpose list.
- `HashSet`: unique values, no ordering guarantee.
- `TreeSet`: unique sorted values.
- `HashMap`: key-value lookup.
- `TreeMap`: sorted keys.
- `ArrayDeque`: efficient deque/stack/queue operations.

## Practice
1. Store and sort student names.
2. Remove duplicates from a list using a set.
3. Count word frequencies with a map.
4. Build a queue simulation.
5. Build a phone-book map.

## Mini assignment
Create a **Student Registry** using `Map<Integer, Student>` with add, search, update, delete and list operations.
