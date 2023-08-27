# Garbage Collection

👆🏽 Performed by JVM

## Generational Collectors

JVM perform garbage collection on objects on basis of their age in the program.

### Heap Memory Division

---

> Young Generation (Eden Space)
>
> Old Generation
>

---

Survivor Space from     |      Survivor to

---

---

<———————————————————Heap ——————————————————>

- Garbage collection steps
  - Objects are stored in Eden space, when they are created at first.
  - When Eden Space gets full
  - 1st cycle
    - Minor GC runs
    - Objects moved to survivor space 1
  - Eden space gets full again
  - 2nd cycle
    - Objects moved to survivor space 2
      from both Eden space and survivor 1

    💡 Objects keep moving between both survivor spaces in cycles

    Objects older than Max tenure threshold (a certain threshold for number of cycles)
    are moved to old generation space.

    - When old generation space is about to be full
    - major GC runs → *time consuming and might pause the application*

## Types of GC

- **Single**
  - Operation

    Stops the application and runs a single thread for garbage collection.

    - Used when

        Suitable for small applications.

- Concurrent
  - Operation
    Runs a GC thread alongside the application.

    - Used when:
      - More memory available
      - High number of CPUs or cores present
      - App demands short pauses

      (Used in most fintech apps)

    (CMS - Concurrent Mark Sweep)

- G1 Garbage Collector

    Introduced in Java 7 to replace CMS

  - Operation
    - No concept of young and old generations
    - Divides Heap into several memory spaces
    - Collects from region which has most garbage → Garbage first (G1)
  - Advantages
    - GC pauses can be tuned
    - Small pauses
    - Parallelism and concurrency together
    - Better heap utilisation

[[Garbage Collection of static variables]]
