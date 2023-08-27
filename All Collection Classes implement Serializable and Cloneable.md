# All Collection Classes implement [[Serializable]] and [[Cloneable]]

- Why though?

    Collections $\equiv$ Containers in C++ → used to transfer

    To transfer object from one place to another, it should be **serializable**.

    When sent from one place to another, the receiver makes a copy of it and operates on it → **clonable**
