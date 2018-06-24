# Numbers

## Integers and Floats
- Ruby numbers has 2 categories: Intergers and Floats.
- Integers is numbers with no decimal points. Ex: 10, -5
- Floats is numbers with decimal points. Ex: 1.25, -3.144445

## Examples:
```ruby
# Integer
x = 10
x.class
=> Integer

# Float
x = 5.0
x.class
=> Float
 
x = 10.25
x.class
=> Float
``` 

## Operaters
- Addition (+)
```ruby
3 + 5   #=> 8
3 + 5.5 #=> 8.5
```

- Substraction (-)
```ruby
5 - 3    #=> 2
3 - 5.5  #=> -2.5
```

- Multiplication (*)
```ruby
3 * 5    #=> 15
3 * 5.5  #=> 16.5
```

- Division (/)
```ruby
10/3    #=> 3
10/3.0  #=> 3.3333333333333335
10.0/3  #=> 3.3333333333333335
```

- To power (**)
```ruby
2**3  #=> 8
```

- Modulo (%)
```ruby
10 % 3  #=> 1
10 % 4  #=> 2
```


## Convert numbers
- Convert to Float: Using to_f
```ruby
x = 5
x.class
=> Integer
x = x.to_f
=> 5.0
x.class
=> Float
```

- Convert to Integer: Using to_i
```ruby
x = 5.3
x.class
=> Float
x = x.to_i
=> 5
x.class
=> Integer
```

- Convert to String: Using to_s
```ruby
500.to_s
=> "500"
10.22.to_s
=> "10.22"
```
