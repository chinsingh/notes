# Java is always Pass [[by Value]]

Whenever a method is invoked in Java, it is allotted its own stack space. Regardless of the original variable type, each time a method is invoked, a copy for each argument is created in the stack memory and the copy version is passed to the method. Thus, always pass by value.

For more details on [[How Arguments are Passed in Java]] see [[How Arguments are Passed in Java]].
