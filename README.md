# Axiom

## Axiom is a simple c-like programming langage. The only big difference is its JavaScript's lyke dynamic typing for **ONLY** values (like a string can be implicitly converted to a double, but a vec3 for example (or any type excepted 'value') **can't** be converted implicitly converted to an other type). 

### Expressions:
- 1+1 will be automaticly converted to **true** for example, like any non-null values if needed.
- {item0, item1, ...} for declaring an array, an array can contain an other.
- (item0, item1, ...} for declaring objects from structures.

### Object declaration:
- {type} {name};
- {type} {name} = {expr};

### Array of objects declaration:
- {type} {name}[{dim0}][{dim1}]...;
- {type} {name}[{dim0}][{dim1}]... = {expr};

### Loops:
#### If:
- if (expr) {statement list}
- if (expr) {statement list} else {statement list}

#### While:
- while (expr) {statement list}

### Declaring a struct:

struct {name}[({parent})] {statement list}
#### statement list can contains:
- Objects declaration
- Functions
