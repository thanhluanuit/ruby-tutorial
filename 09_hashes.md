# Hashes

A Hash is a dictionary - like collection of key-value pairs.

## Examples:

```ruby
ages   = { "Tony" => 22, "KenJ" => 25 }
months = { 1 => "January", 2 => "February", 3 => "March" }
attrs  = { :font_size => 22, :color => "red" }
```

## Retrieves value by key
```ruby
ages = { "Tony" => 22, "KenJ" => 25 }

ages["Tony"]
=> 22
ages["KenJ"]
=> 25
```

```ruby
months = { 1 => "January", 2 => "February", 3 => "March" }

months[1]
=> "January"
months[2]
=> "February"
months[3]
=> "March"
months[4]
=> nil #  meaning “nothing”
```

```ruby
attrs  = { :font_size => 22, :color => "red" }

attrs[:font_size]
=> 22
attrs[:color]
=> "red"
```

## Common Uses
```ruby
# Create a blank hash and Add elements to hash
profile = {} 
profile[:user_name] = "Tony"    
profile[:language]  = "English" 
profile[:age] = 25     

profile
=> {:user_name => "Tony", :language => "English", :age => 25}

# Get list keys
profile.keys 
=> [:user_name, :language, :age]

# Get list values
profile.values
=> ["Tony", "English", 25]

# Retrieves value by key
profile[:user_name]
=> "Tony" 
```

## Noted
- Remember that *keys in a hash are unique*.
- Recommend using Symbols as Hash Keys
