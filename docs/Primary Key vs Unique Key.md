# [[Primary Key]] vs [[Unique Key]]

|                | Primary Key                                                                 | Unique Key                                                                                              |
|----------------|-----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
| Basic          | Used to serve as a unique identifier for each row in a table                | Uniquely determines a row which isn't primary key                                                       |
| NULL value     | Can't be NULL                                                               | Can accept one NULL value. If it accepts two -> no longer unique.                                       |
| Number of keys | Be it made of one or many attributes, but there can only be one primary key | There can be multiple unique keys either made of a single attribute or multiple attributes put together |
| Index          | Creates a [[clustered index]]                                                   | Creates a non-clustered index             |
