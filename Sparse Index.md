# Sparse Indexing

- When you don't store keys of each and every record in the table.
- This can further reduce the size of index table.
- Example
  - You can store every 10 records. Thus you'll have 1, 11, 21, 31, 41., 51... in your index table.
  - Now if you want to search for record number 35 — You know it lies between 31 and 41. Search within the block which has record no. 31.
