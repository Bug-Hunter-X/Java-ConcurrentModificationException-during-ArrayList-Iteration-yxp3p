# Java ConcurrentModificationException Example

This repository demonstrates a common Java error: the `ConcurrentModificationException`.  The `ConcurrentModificationExceptionExample.java` file shows code that throws this exception.  The solution, `ConcurrentModificationExceptionSolution.java`, provides a corrected version using an Iterator for safe list modification during iteration.

The exception arises from modifying a collection (like an ArrayList) while iterating over it using a for-each loop or similar constructs. This is because these methods create an internal iterator, and modifying the list directly invalidates that iterator, leading to the exception.

This example highlights the importance of using appropriate methods for concurrent modifications to collections when using Java's collections framework. Using iterators (as shown in the solution) prevents this common problem.