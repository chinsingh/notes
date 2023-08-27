# Dense Indexing

- When you store keys for each and every value in your index table.
- This may increase the size of your index table, but its not always bad.
- If your database table is unsorted, you won't be able to search based on few records. You'll then need to store block pointers for each and every record.
