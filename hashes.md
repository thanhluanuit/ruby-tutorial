# Hashes

A Hash is a dictionary - like collection of key-value pairs.

## Examples:

```ruby
ages   = { "Tony" => 22, "KenJ" => 25 }
months = { 1 => "January", 2 => "February", 3 => "March" }
attrs  = { :font_size => 22, :color => "red" }
```

## Create a Hash

```ruby
# Create a new empty hash
profile = {} 

# Add new elements to hash
profile[:user_name] = "Tony"    
profile[:language]  = "English" 
profile[:age]       = 25     

profile
=> {:user_name => "Tony", :language => "English", :age => 25}
```

## Accessing value by key
```ruby
ages = { "Tony" => 22, "KenJ" => 25 }

ages["Tony"] #=> 22
ages["KenJ"] #=> 25
```

```ruby
months = { 1 => "January", 2 => "February", 3 => "March" }

months[1]   #=> "January"
months[2]   #=> "February"
months[3]   #=> "March"
months[4]   #=> nil
```

```ruby
attrs = { :font_size => 22, :color => "red" }

attrs[:font_size]  #=> 22
attrs[:color]      #=> "red"
```

## Common Uses
```ruby
profile = {:user_name => "Tony", :language => "English", :age => 25}
```

- Get list keys

```ruby
profile.keys 
=> [:user_name, :language, :age]
```

- Get list values

```ruby
profile.values
=> ["Tony", "English", 25]
``` 

## Iteration
### each
You can iterate over keys and values

```ruby
{x: 1, y: 2, z: 3}.each do |key, value|
  puts "key: #{key} and value: #{value}"
end

# Output
key: x and value: 1
key: y and value: 2
key: z and value: 3
```

### each_with_index

```ruby
{x: 3, y: 4, z: 5}.each_with_index do |(key, value), index| 
  puts "Index #{index}: key is #{key} and value is #{value}"
end

# Output
Index 0: key is x and value is 3
Index 1: key is y and value is 4
Index 2: key is z and value is 5
```

## Filtering with *select*, *reject*
- *select* 

```ruby
hash = {:a => 1, :b => 2, :c => 3}
hash.select{|key, value| value.even?}   
=> {:b=>2}
```

- *reject*

```ruby
hash = {:a => 1, :b => 2, :c => 3}
hash.reject{|key, value| value.even?}   
=> {:a=>1, :c=>3}
```

## Noted
- Remember that *keys in a hash are unique*.
- Recommend using Symbols as Hash Keys
