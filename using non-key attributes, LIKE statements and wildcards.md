# using non-key attributes, LIKE statements and wildcards

- Using non-key attributes, LIKE statements and wildcards.
- Since most databases create primary index on their own, it doesn't take much time to search based on keys. If you go searching for non-key attributes, the database will have to go for a sequential search.
- Or worse, if you go for wildcards. Now, not only it has to sequentially search, but also match all values to your wildcard.
- If there are going to be some non-key values you'll frequently use, it is better in most cases to maintain a [[Secondary Index]] on those values.

## References

[Database Indexing Explained (with PostgreSQL) - Hussein Nasser](https://youtu.be/-qNSXK7s7_w)
