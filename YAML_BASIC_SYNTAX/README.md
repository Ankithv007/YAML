## YAML Structure

YAML uses indentation to represent data hierarchy and organizes content in a clear and readable way. Below are some common structures in YAML:

### Scalars
Simple values such as strings, numbers, and booleans.
```yaml
name: John Doe
age: 30
is_student: false
```

### Lists
Sequences are represented using a dash (`-`) followed by a space.
```yaml
fruits:
  - Apple
  - Banana
  - Cherry
```

### Dictionaries
Mappings are represented using `key: value` pairs.
```yaml
person:
  name: John Doe
  age: 30
  city: Bangalore
```

### Nested Structures
Combining lists and dictionaries to form complex hierarchies.
```yaml
company:
  name: Tech Solutions
  employees:
    - name: Alice
      role: Developer
    - name: Bob
      role: Manager
  locations:
    head_office:
      city: Bangalore
      country: India
    branch_office:
      city: Pune
      country: India
```
## YAML Data Types

YAML supports a variety of data types for different use cases:

1. **String**
   - Single-line or multi-line text.
   - Example:
     ```yaml
     message: "Hello, World!"
     description: |
       This is a multi-line string.
       It spans multiple lines for better readability.
     ```

2. **Number**
   - Can be integers or floating-point numbers.
   - Example:
     ```yaml
     age: 25
     temperature: 36.6
     ```

3. **Boolean**
   - Represents true or false values.
   - Example:
     ```yaml
     is_active: true
     is_admin: false
     ```

4. **Null**
   - Represents the absence of a value.
   - Example:
     ```yaml
     middle_name: null
     ```

5. **Lists**
   - Ordered collections of items.
   - Example:
     ```yaml
     colors:
       - Red
       - Green
       - Blue
     ```

6. **Dictionaries (Mappings)**
   - Unordered collections of key-value pairs.
   - Example:
     ```yaml
     address:
       street: "123 Main St"
       city: "Bangalore"
       zip: "560001"
     ```