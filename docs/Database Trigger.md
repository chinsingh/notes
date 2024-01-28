# Database Trigger

Piece of procedural code that is automatically executed in response to a specific event occurring within a database. The event can be data manipulation event like insert, delete or update, or it could be a system event like login/logout.

The trigger code can perform a variety of actions, such as updating other tables, enforcing business rules, or logging information. The trigger code has access to the data that caused the trigger to fire, as well as to any other data in the database.

## Types

- Row-level triggers: Fired once for each row affected by the data manipulation.
- Statement-level triggers: Fired once for each statement performing some data manipulation.

## Creating triggers

Triggers can be created via some database management tool or via SQL commands.

For example -
```sql
CREATE TRIGGER update_customer_status
AFTER INSERT ON orders
FOR EACH ROW
BEGIN
UPDATE customers
SET customer_status = 'Active'
WHERE customer_id = NEW.customer_id;
END;
```

## Best Practices

Triggers can performance issues if not used properly.

- Keep triggers simple and efficient. Avoid running complex or resource-intensive code in triggers.
- Test triggers thoroughly before deploying them to a production environment.
- Avoid creating triggers that modify the same data that triggered them, as this can cause an infinite loop.
- Document your triggers thoroughly so that other developers can understand their purpose and functionality.

## References

[A Beginner's Guide to Database Triggers](https://medium.com/@cfqbcgwkg/a-beginners-guide-to-database-triggers-dc238e7bceb)
