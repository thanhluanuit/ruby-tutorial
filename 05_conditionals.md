# Conditionals

## if

```ruby
if expression 
  code
end
```
The code between *if* and *end* is executed when the *expression* evaluates to true.

Examples:
```ruby
# If x is greater than 5, increment x
x = 6 
if x > 5
  x += 1
end
x #=> 7


if 10 > 5
  puts "10 is greater than 5"
end
```

## else
An *if* statement can include an **else** clause to specify code to be executed if the condition is not true:

```ruby
if expression 
  code
else
  code
end
```

Examples:

```ruby
a = 10
b = 5

if a > b
  puts "#{a} is greater than #{b}"
else
  puts "#{b} is greater than #{a}"
end
```

## elsif
elsif is a shortened form of "else if"

```ruby
if expression_1
  code
elsif expression_2
  code
  .
  .
elsif expression_n
  code
else
  code
end
```

Examples:
```ruby
if month < 6
  price *= 0.8  # sale of 20%
elsif month == 6
  price *= 0.7  # sale of 30%
else # months in 7..12
  price *= 0.9  # sale of 10%
end
```

## unless

```ruby
unless expression 
  code
end
```
Same with:
```ruby
if !expression
  code  
end
```
- *unless* is the opposite of *if*. 
- *unless* executes code when expression evaluates to *false* or *nil*. 

Examples:
```ruby
x = 3
unless x > 5   # That mean when x not greater than 5
  x += 1       # Increment x
end
```


## case
*case* expression is an alternative to the if-elsif-else expression.

Examples:

```ruby
score = 9

case score
when 1..4
  puts "Failed!"
when 5
  puts "Pass!"
when 6..7
  puts "Not bad!"
when 8..10
  puts "Excellent!"
else
  puts "Invalid score."
end
```

```ruby
date = 5

case date
when 2,4,6
  puts "Working in the morning" 
when 3,5,7
  puts "Working in the afternoon"
else
  puts "Off" 
end
```
