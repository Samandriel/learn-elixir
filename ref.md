# Definitions
- **Immutability:** In Elixir, once a variable references a list such as [1,2,3], you know it will always reference those same values (until you rebind the variable). The value cannot be changed, but we can copy the value, modify it then bind it to a new variable.
- **Module:** collection of different methods or functions
```
defmodule Cards do
    ...
end
```
- **Implicit Return:** Whatever in the last line of inside method or function will be a return value by default.
```
def hello do
    ...
    ...
    "Hi there!"
end
```
- **Explicit Return:**
```
def hello do
    ...
    ...
    return "Hi there!"
end
```
- **Method Argument** Any value that pass to a method.
```
def shuffle(deck) do
    ...
en
```



- ****

---
