# HashMap

implements [[Map]]

## Initialization

```java
Map map = new HashMap();
```

or

```java
Map<String, String> map = new HashMap<String, String>();
```

## Methods

- `map.put("key", "value");`
- `map.get("key");` → value
- `keySet()` → Set of keys

What happens when Repeating/duplicate keys ⇒ value gets replaced

- Fixed Order insertion → Linked HashMap
- Sorting Order → Tree HashMap

[[HashMap Implementation]]
