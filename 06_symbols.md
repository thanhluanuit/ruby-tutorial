# Symbols

- A symbol is written by prefixing an a word with a colon.
- Symbols often used as keys in Hashes (see in next section) 

## Examples

```ruby
:age
:"age"
:name
```

## Common Uses
- Convert a string to symbol (to_sym) 
    ```ruby
    animal = "dog"
    animal.to_sym
    => :dog
    ```

- Convert a symbol to string (to_s)
    ```ruby
    animal = :dog
    animal.to_s
    => "dog" 
    ```
