- A top level class is a class that is not a nested class.
  A nested class is any class whose declaration occurs within the body of another class or interface.
  An inner class is a nested class that is not explicitly or implicitly declared static

- Inner classes can declare a static members only if it is a constant (i.e. final).

- When a connection is created with JDBC, it is in auto-commit mode. i.e. auto-commit is enabled. This means that each individual SQL statement is treated as a transaction and is automatically committed right after it is completed. (A statement is completed when all of its result sets and update counts have been retrieved. In almost all cases, however, a statement is completed, and therefore committed, right after it is executed.) The way to allow two or more statements to be grouped into a transaction is to disable the auto-commit mode. Since it is enabled by default, you have to explicitly disable it after creating a connection by calling con.setAutoCommit(false);

-
