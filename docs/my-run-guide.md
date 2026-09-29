# Run the library demo

## Prerequisites

- Git 2.23 or newer to clone and work with the repository.
- Python 3.9 or newer.
- JDK 17 or newer, with both `java` and `javac` available on `PATH`.

Open a terminal in the repository root, where `run.py` is located, then run:

```sh
python3 run.py demo
```

On Windows, use `py -3 run.py demo` or `python run.py demo` if that is your Python 3 command.
No Maven, external Java libraries, or separate build step is needed. The runner compiles the Java sources in a temporary directory and cleans it up afterward.

The demo creates three catalog books and student/faculty members, prints their borrowing limits and the result of searching for `git`, then borrows and returns Git Essentials for Alex. It prints the receipt, due date, return fee, and remaining active loans. The date is fixed at 2026-09-01 so the result is reproducible. Baseline title search is case-sensitive, so the lowercase query `git` does not match `Git Essentials`.
