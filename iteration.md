# Iteration


## *each* 

### In Arrays
You can iterate elements in array:

```ruby
[3, 4, 5].each{ |i| puts "element: #{i}" }
```
Output:

```ruby
element: 3
element: 4
element: 5
```

You can iterate over nested arrays:
```ruby
[[1, 2], [3, 4], [7, 8]].each do |a, b| 
  puts "a: #{a}, b: #{b}" 
end
```
Output:
```ruby
a: 1, b: 2
a: 3, b: 4
a: 7, b: 8
```

### In Hashes
You can iterate over keys and values
```ruby
{x: 1, y: 2, z: 3}.each do |key, value|
  puts "key: #{key} and value: #{value}"
end
```
Output
```ruby
key: x and value: 1
key: y and value: 2
key: z and value: 3
```


## *for* iterator

```ruby
months = ["January", "February", "March", "April", "May", "June"]
for month in months
  puts month
end
```
Output
```ruby
January
February
March
April
May
June
```

```ruby
for i in 5..10
  puts i
end
```
Output
```ruby
5
6
7
8
9
10
```

## Iteration with index: *each_with_index*

### In Arrays
```ruby
[3, 4, 5].each_with_index do |element, index|
  puts "Index #{index}: element is #{element}"
end
```
Output
```ruby
Index 0: element is 3
Index 1: element is 4
Index 2: element is 5
```

### In Hashes
```ruby
{x: 3, y: 4, z: 5}.each_with_index do |(key, value), index| 
  puts "Index #{index}: key is #{key} and value is #{value}"
end
```
Output
```ruby
Index 0: key is x and value is 3
Index 1: key is y and value is 4
Index 2: key is z and value is 5
```


## *map*

Return the changed object, but original object remains.

```ruby
arr = [3, 4, 5]
arr.map{ |i| i * 2 }  #=> [6, 8, 10]
arr #=> [3, 4, 5] 
```

*map!* changes the original object

```ruby
arr = [3, 4, 5]
arr.map!{ |i| i * 2 }  #=> [6, 8, 10]
arr #=> [6, 8, 10]
```
