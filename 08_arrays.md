# Arrays

Array is a collection that can be used to store a list of values.

## Create an Array
```ruby
array_1 = [1, 2, 5, 10, 9, 7]
array_2 = ["hello", "welcome", "array", "Ruby"]

array_3 = []
array_3 << 1 # Insert 1 to array_3
array_3 << 2 # Insert 2 to array_3
array_3 << 3 # Insert 3 to array_3
=> [1, 2, 3]
```

## Index

```ruby
Array: [5, 2, 4, 7, 9]
        |  |  |  |  |
Index:  0  1  2  3  4
```
That mean: The first element gets the index 0. The second gets 1, and so on.

```ruby
array = [5, 2, 4, 7, 9]
array[0] # => 5 
array[1] # => 2 
array[4] # => 9
```

## Common methods
- Get first element in array
```ruby
array = [5, 2, 4, 7, 9]
array[0]    # => 5
array.first # => 5

```

- Get last element in array
```ruby
array = [5, 2, 4, 7, 9]
array.last # => 9
array[4]   # => 9
array[-1]  # => 9
```

- Get second of last element in array
```ruby
array = [5, 2, 4, 7, 9]
array[-2]  # => 7
```

- Check a particular value in array
```ruby
array = [5, 2, 4, 7, 9]

array.include?(4)
=> true

array.include?(1)
=> false

array.include?("hello")
=> false
```
