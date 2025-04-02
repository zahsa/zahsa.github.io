
# Dictionary
- key-value pairs, unordered (the elements are not stored in any specific order), mutable (you can modify their contents after creation)
- elements go inside {}

# Set
- Unordered, mutable, no duplicates
- elements go inside {}

# List
- Ordered (the order in which the elements are defined is preserved), mutable
- Used when the data might need to be modified (e.g., adding/removing items).
- elements go inside []
- Lists are better suited for tasks that involve iteration and changing data over time.

Methods:

- append(item): Adds an item to the end of the list.

- insert(index, item): Inserts an item at a specific index.

- remove(item): Removes the first occurrence of item.

- pop(): Removes and returns the last item.

- extend(iterable): Extends the list by appending all the items from another iterable.

- sort(): Sorts the list in place.

# Tuple
- immutable (once a tuple is created, its elements cannot be changed, added, or removed), ordered
- Storing multiple items including strings and numerical values
- Unchangable (immutable), allows duplicates
- elements go inside ()

Methods:
- count(value): Counts occurrences of value in the tuple.
  
- index(value): Returns the index of the first occurrence of value.

# Examples
my_tuple = tuple(["Max", 28, "Boston"])  
my_dict = dict(name = "Mary", age = 27)  
my_set_1 = set([1,2,3])  
my_set_2 = set("hello")  
my_list = [1, 2, 3]
