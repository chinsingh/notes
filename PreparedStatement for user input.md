# PreparedStatement for user input

Use PreparedStatement instead of Statement to give user input in queries

query - (?,?) // question marks for parameters you want to take as user input in the query

```java
Prepared Statement st = con.prepareStatement(query); 
st.setInt(1, input1); 
st.setString(2, input2);
```
