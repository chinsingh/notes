# Indexing

To make retrieving from a database table faster, we split database table into blocks, make a separate table (index) similar to indexes in a book, which stores the search key and the block pointer (address of the first record in block).

## Explanation

- Suppose you write a book with 10,000 lines.
- 10,000 lines was a lot so you split it up into 1000 pages. 10 line per page.
- Similarly, database tables can be split up into blocks.
- Time taken to search within a page/block is negligible
- Ways to search this book/split-up database — find line no. /record no. 945
  - If the book/database is sorted
    - Binary search
  - If the book/database is unsorted
    - Linear search
- Either way, you'll have to visit a lot of records individually
- A better way would be to create an index.
- Since here we're using line/record number to search, we create an index on line/record numbers.
- This index will mention the record number and its page number.
- Now you can simply go through this table, directly go to the page number and find the record.

Only works if index table is significantly smaller than the database table. → Index tables don't contain the complete records, just the key and pointer.
