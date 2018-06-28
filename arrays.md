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

## Indexing
- Array indexing start at 0 for first element, the second gets 1, and so on.
- An index of -1 indicates the last element of the array, -2 is the next to last element in the array, and so on.

```ruby
Array: [5, 2, 4, 7, 9]
        |  |  |  |  |
Index:  0  1  2  3  4
```

```ruby
array = [5, 2, 4, 7, 9]
array[0]  # => 5 
array[1]  # => 2 
array[4]  # => 9
array[-1] # => 9
```

## Accessing elements

- Get first element in array

```ruby
array = [5, 2, 4, 7, 9]
array[0]     # => 5
array.first  # => 5
```

- Get last element in array

```ruby
array = [5, 2, 4, 7, 9]
array.last  # => 9
array[4]    # => 9
array[-1]   # => 9
```

- Get second of last element in array

```ruby
array = [5, 2, 4, 7, 9]
array[-2]  # => 7
```

- Get first n elements in array

```ruby
array = [5, 2, 4, 7, 9]
array.first(3)  # => [5, 2, 4]
```

- Get last n elements in array

```ruby
array = [5, 2, 4, 7, 9]
array.last(2)  # => [7, 9]
```

## Iteration
### each

You can iterate elements in array:

```ruby
[3, 4, 5].each{ |i| puts "element: #{i}" }
# Output:
element: 3
element: 4
element: 5
 => [3, 4, 5]
```

You can iterate over nested arrays:

```ruby
[[1, 2], [3, 4], [7, 8]].each do |a, b| 
  puts "a: #{a}, b: #{b}" 
end
# Output:
a: 1, b: 2
a: 3, b: 4
a: 7, b: 8
 => [[1, 2], [3, 4], [7, 8]]
```

### each_with_index
You can iterate elements with index in array:

```ruby
[3, 4, 5].each_with_index do |element, index|
  puts "Index #{index}: element is #{element}"
end
# Output
Index 0: element is 3
Index 1: element is 4
Index 2: element is 5
```

## Filtering with *select*, *reject*

- *select*: will returen elements match to the condition

```ruby
array = [5, 2, 4, 7, 9]
array.select{|item| item > 5} # => [7, 9]
```

- *reject*: will returen elements do not match to the condition

```ruby
array = [5, 2, 4, 7, 9]
array.reject{|item| item > 5} # => [5, 2, 4]
```

## map: 
Create new array by invoke a block on each element of array.

```ruby
array = [1, 2, 3]
array.map{|item| item * 2}  # => [2, 4, 6]
array.map{|item| item.to_s} # => ["1", "2", "3"]
array.map(&:to_s)           # => ["1", "2", "3"]
```

## Common methods

- Count numbers of elements of array with #count, #length or #size

```ruby
array = [1, 2, 4, 7, 9]
array.count    # => 5
array.length   # => 5
array.size     # => 5
```

- Remove all nil elements in array with #compact and #compact!

```ruby
array = [5, nil, 4, 7, 9, nil]
# It return new copy array with nil removed
# Without effecting the origin array
array.compact    #=> [5, 4, 7, 9]
array            #=> [5, nil, 4, 7, 9, nil]

# It effect to origin array
array.compact!   #=> [5, 4, 7, 9]
array            #=> [5, 4, 7, 9]
```

- Check a particular value in array with #include?

```ruby
array = [5, 2, 4, 7, 9]
array.include?(4)
=> true

array.include?(1)
=> false

array.include?("hello")
=> false
```
