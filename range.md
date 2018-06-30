# Range

## What is a Range?

- A range is a sequence of values with a beginning and an end.
- A range is look like a variation of an array.
- The values in a range can be numbers, characters, strings or objects. 
- Examples: 0 to 9, 'a' to 'z', January to December, ...

## Create a Range

Ruby uses 2 operators are **..** and  **...** to generate a range.

#### Syntax

```ruby
(begin..end)  #=> will include the end value 
(begin...end) #=> will exclude the end value
```

#### Example

```markdown
(9..1).to_a     #=> []
(1..9).to_a     #=> [1, 2, 3, 4, 5, 6, 7, 8, 9] - (inclusive 9)
(1...9).to_a    #=> [1, 2, 3, 4, 5, 6, 7, 8]    - (exclusive 9)

('a'..'h').to_a  # => ["a", "b", "c", "d", "e", "f", "g", "h"]
('a'...'h').to_a # => ["a", "b", "c", "d", "e", "f", "g"]
``` 


## Iteration

```ruby
(1..5).each do |i|
  puts i
end
# Print 
1
2
3
4
5
```

```ruby
require 'date'

date1 = Date.new(2018, 8, 1)
date2 = Date.new(2018, 8, 5)

(date1..date2).each do |date| 
  puts date
end
# Print 
2018-08-01
2018-08-02
2018-08-03
2018-08-04
2018-08-05
```

## Common methods

- Check a element in arange: *include?(obj)*

```ruby
("a".."z").include?("n")   #=> true
("a".."z").include?("N")   #=> false
(1..9).include?(10)        #=> false
```

```ruby
require 'date'
date1 = Date.new(2018, 8, 1)
date2 = Date.new(2018, 8, 5)
(date1 .. date2).include?(Date.new(2018, 8, 3))  #=> true
```

- First and first n elements in a range

```ruby
(1..100).first    # => 1
(1..100).first(5) # => [1, 2, 3, 4, 5] 
```

- Last and last n elements in a range

```ruby
(1..100).last     # => 100
(1..100).last(10) # => [91, 92, 93, 94, 95, 96, 97, 98, 99, 100] 
```

- Get number of elements in a range

```ruby
(1..100).size     # => 100
```
