# [[HashMap]] vs [[Hashtable]]

|               | HashMap                                                        | Hashtable                                                 |
|---------------|----------------------------------------------------------------|-----------------------------------------------------------|
| Introduced in | 1.2                                                            | 1.0                                                       |
| Thread Safety | Not thread safe (not synchronized) => works with single thread | Thread safe (synchronized) => works with multiple threads |
| Speed         | Faster                                                         | Slower                                                    |
| Null key      | One null key allowed                                           | Null key not allowed                                      |
