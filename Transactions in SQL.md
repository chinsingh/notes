# Transactions in SQL

## BEGIN TRANSACTION

Indicates start point of an explicit or local transaction.

```sql
BEGIN TRANSACTION transaction_name ;
```

## SET TRANSACTION

```sql
SET TRANSACTION [READ WRITE | READ ONLY] ;
```

## COMMIT

Used to save all the changes since the last commit/rollback if everything is in order.

```sql
COMMIT;
```

## ROLLBACK

Used to rollback all changes since last commit or rollback.

```sql
ROLLBACK;
```

## SAVEPOINT

Creates a point in the transaction to rollback to without rolling back the entire transaction.

```sql
SAVEPOINT savepoint_name;
```

```sql
ROLLBACK TO savepoint_name;
```

## RELEASE SAVEPOINT

Used to remove a savepoint.

```sql
RELEASE SAVEPOINT savepoint_namel;
```
