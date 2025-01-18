# YAML: Advanced Data Types

YAML offers several advanced data types for handling complex scenarios and enabling better data organization. Below is an overview of these data types, including examples and use cases.

---

## 1. Timestamps
YAML can represent dates and times in standard ISO 8601 format.

### Syntax
```yaml
# ISO 8601 format
created_at: 2025-01-18T14:30:00Z
updated_at: 2025-01-18T15:45:00+05:30

# Date only
start_date: 2025-01-18
```

### Use Case
For tracking logs, events, or metadata in a structured and easily parseable manner.

---

## 2. Null
Represents the absence of a value.

### Syntax
```yaml
missing_value: null  # Explicit
not_provided:        # Implicit
```

### Use Case
Indicating optional fields or placeholders for data yet to be added.

---

## 3. Booleans
YAML supports `true` and `false` as boolean values.

### Syntax
```yaml
is_active: true
is_verified: false
```

### Use Case
For binary states such as flags, toggles, or configuration switches.

---

## 4. Floats and Integers
YAML supports various number formats, including scientific notation for floats.

### Syntax
```yaml
# Integers
quantity: 42
hex_value: 0x2A  # Hexadecimal

# Floating-Point Numbers
price: 199.99
scientific: 4.2e1  # Equivalent to 42
infinity: .inf
not_a_number: .nan
```

### Use Case
For numerical data, prices, or statistics.

---

## 5. Binary Data
Binary content can be represented using Base64 encoding.

### Syntax
```yaml
image_data: !!binary |
  R0lGODdhEAAQAMQAAORHHOVGHOVOHuVRHuVPHuVTHvVXHvVbHvVfHvVjHvVnHvVrHvVvHvVzHvV3HvV7HvV/
```

### Use Case
Embedding small binary data (e.g., images, files) directly within the YAML document.

---

## 6. Merged Dictionaries
Allows combining dictionaries using the `<<` key with anchors and aliases.

### Syntax
```yaml
default_settings: &default
  timeout: 30
  retries: 3

custom_settings:
  <<: *default
  timeout: 60
```

### Output
```yaml
custom_settings:
  timeout: 60
  retries: 3
```

### Use Case
Reusing or overriding configuration blocks without duplicating data.

---

## 7. Sets
Represents a unique collection of values.

### Syntax
```yaml
unique_items: !!set
  ? Item1
  ? Item2
  ? Item3
```

### Use Case
For data where duplicates are not allowed, such as tags or unique attributes.

---

## 8. Ordered Mappings
YAML can enforce ordering for dictionaries using the `!!omap` tag.

### Syntax
```yaml
ordered_dict: !!omap
  - key1: value1
  - key2: value2
  - key3: value3
```

### Output
```
{
  "key1": "value1",
  "key2": "value2",
  "key3": "value3"
}
```

### Use Case
When the order of keys in a mapping is significant.

---

## 9. Pairs
Represents key-value pairs as a sequence.

### Syntax
```yaml
pairs: !!pairs
  - [key1, value1]
  - [key2, value2]
```

### Use Case
For use cases involving pair relationships, such as defining edges in graphs.

---

## Summary
Advanced data types in YAML enable versatile and robust data representation. These include timestamps for temporal data, sets for unique collections, binary for encoding, and merged dictionaries for configuration management. Using these types appropriately can significantly improve data clarity and usability.
