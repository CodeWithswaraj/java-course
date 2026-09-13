# Lesson 15 — Multithreading & Concurrency

## Learning objectives
Understand threads, tasks, synchronization, executors and common concurrency problems.

## Creating a thread
```java
class Worker extends Thread {
    @Override
    public void run() {
        System.out.println("Working...");
    }
}

new Worker().start();
```

Prefer task-based APIs such as executors for real applications.

## Runnable
```java
Runnable task = () -> System.out.println("Task running");
new Thread(task).start();
```

## Race condition
When multiple threads access shared mutable state without correct coordination, results can become unpredictable.

## synchronized
```java
synchronized void increment() {
    count++;
}
```
Use synchronization deliberately; understand its scope and cost.

## ExecutorService
```java
ExecutorService pool = Executors.newFixedThreadPool(2);
pool.submit(() -> System.out.println("Task"));
pool.shutdown();
```

## Modern concurrency topics
Learn `Future`, `Callable`, concurrent collections, locks, atomics, `CompletableFuture` and virtual threads after mastering the fundamentals.

## Practice
1. Run two threads with different messages.
2. Demonstrate a race condition.
3. Fix it using synchronization.
4. Submit tasks to an executor.
5. Return a result with `Callable` and `Future`.

## Mini assignment
Build a **parallel file word counter** that processes multiple text files using an executor and combines the results safely.
