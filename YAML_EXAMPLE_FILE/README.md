# Complete YAML Example

Here is a complete YAML file example demonstrating various features like scalars, lists, dictionaries, and nested structures:

```yaml
# Basic Information
name: John Doe
age: 30
is_active: true

# Contact Details
contact:
  email: john.doe@example.com
  phone:
    - type: home
      number: "123-456-7890"
    - type: work
      number: "987-654-3210"

# Skills and Expertise
skills:
  - name: Programming
    proficiency: Expert
    languages:
      - Python
      - JavaScript
      - Java
  - name: DevOps
    proficiency: Intermediate
    tools:
      - Docker
      - Kubernetes
      - Jenkins

# Employment History
employment_history:
  - company: Tech Solutions
    role: Software Engineer
    duration: 3 years
    projects:
      - name: E-commerce Platform
        description: "Developed a scalable online shopping application."
      - name: Inventory System
        description: "Designed an automated inventory management tool."
  - company: Cloud Innovators
    role: DevOps Engineer
    duration: 2 years
    responsibilities:
      - Setting up CI/CD pipelines
      - Managing Kubernetes clusters
      - Ensuring infrastructure security

# Preferences
preferences:
  preferred_work_location: Remote
  relocation_willingness: false
  hobbies:
    - Hiking
    - Reading
    - Traveling

# Comments and Notes
notes: |
  This is a sample YAML file.
  It demonstrates key YAML features such as hierarchical structures and lists.
  Use it as a template for your YAML configurations.
```

