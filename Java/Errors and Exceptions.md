In Java, errors and exceptions are differentiated based on their severity, recoverability, and how they are handled in the code.
#### Errors
  * **Errors** are *unrecoverable issues* that signify serious problems during program execution. These are typically caused by external factors like *out-of-memory situations or system crashes.* Examples include OutOfMemoryError and StackOverflowError.
 * **OutOfMemoryError**: Occurs when the program tries to allocate more memory than the system can provide.
 * **StackOverflowError**: Arises when function calls exceed the available stack memory, often due to excessive recursion.
 * **ClassFormatError**: Indicates a problem with the structure of a class file, preventing the program from loading the class.
 * **ThreadDeathError**: Signals an unrecoverable thread termination initiated by the Java Virtual Machine (JVM).
#### Exceptions
 * **Exceptions** are recoverable events that interrupt the normal program flow due to issues *within the program's control,* like *division* *by zero* or *null pointer access*. Exceptions can be handled using try-catch blocks to provide alternative execution paths. Common examples include ArithmeticException, NullPointerException, and ArrayIndexOutOfBoundsException.
 * Java exceptions can be broadly classified into two categories: *checked and unchecked.*
 * **Checked Exceptions:** These exceptions are enforced by the compiler to be *handled explicitly using try-catch* blocks or throws declarations. They are typically related to **potential issues that may arise** during program execution, such as file input/output or network errors.
 * **Types**:
   * **IOException**: Thrown when there's an issue with file input/output operations, like opening a non-existent file.
   * **SQLException**: Indicates an error while interacting with a database, such as connection failure or invalid SQL syntax.

 * **Unchecked Exceptions:** These exceptions are *not checked by the compiler* and can occur due to programming errors or runtime issues like division by zero or null pointer access. They don't require mandatory handling but can *cause abrupt program termination if not addressed*.
 * **Types**:
   * **ArithmeticException**: Occurs when performing mathematical operations like division by zero.
   * **NullPointerException**: Thrown when attempting to use a null object reference.
   * **ArrayIndexOutOfBoundsException**: Arises when trying to access elements outside the bounds of an array.
   
 