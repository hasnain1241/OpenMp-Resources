
#  OpenMP Basics: A Learning Resource


---

##  Overview

This repository provides a **beginner-friendly collection of OpenMP examples** for learning and practicing **parallel programming in C/C++**.

Each example demonstrates a specific OpenMP pragma or concept, making it easier to grasp:

* How OpenMP works
* How to use OpenMP pragmas correctly
* When and why different constructs are used

---

##  Contents

| File / Topic            | Description                                               |
| ----------------------- | --------------------------------------------------------- |
| `parallel_hello.c`      | First parallel program using `#pragma omp parallel`       |
| `parallel_for.c`        | Demonstrates `#pragma omp for` with loop iterations       |
| `static_schedule.c`     | Explains scheduling with `schedule(static)`               |
| `lastprivate_example.c` | Shows how `lastprivate` captures the last iteration value |
| `critical_section.c`    | Prevents race conditions using `#pragma omp critical`     |
| `reduction_example.c`   | Shows reduction of a variable across threads              |
| `nested_parallelism.c`  | Demonstrates nested `#pragma omp parallel` blocks         |

---

##  How to Compile and Run

All examples require OpenMP support. Compile using `gcc` or `g++` with `-fopenmp`:

```bash
gcc filename.c -fopenmp -o output
./output
```

Example:

```bash
gcc parallel_hello.c -fopenmp -o hello
./hello
```

---

---

##  Learning Outcomes

* Understand the basics of OpenMP thread creation and management
* Learn how to parallelize loops effectively
* Avoid race conditions using synchronization techniques
* Practice with real examples for hands-on learning

---

##  Additional Tips

* Use `omp_get_thread_num()` to identify thread IDs.
* Try different `schedule()` policies like `dynamic`, `guided`, or `runtime`.
* Experiment with `private`, `firstprivate`, and `shared` clauses.
* Use `export OMP_NUM_THREADS=4` to control number of threads at runtime.

---

##  License

This is an open educational resource. Free to use for learning and teaching purposes.

---
