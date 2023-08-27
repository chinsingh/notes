# Using the Objects (through its reference variables)

```java
Class Example 
 {
 public static void main(String[] args)
  {
   Box smallBox=new Box();
   smallBox.setDimension(12,10,5);  
   smallBox.showDimension; 
  /*From the perspective of C++, 
  it looks like smallBox is the name of an object. 
  Though its not.*/
   
   smallBox= new Box();
  /*smallBox will now refer to a new object 
  and the older object will become ‘Garbage Block’, 
  which will get destroyed 
  when Garbage collector will run.*/

  smallBox.showDimension();
  /*Will print 0,0,0 since no value is assigned. 
  The default value is 0.*/
  }
}
```
