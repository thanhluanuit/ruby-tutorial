# Constants

## What is a constant?
- It like variables, except its value is supposed to remain constant for the duration of program.
- Constants start with an uppercase letter.

## Example:
```ruby
WELCOME     = 'Welcome to constants'  #=> constant (Recommended)
My_constant = 1000                    #=> constant
SPEED_CAR   = 60                      #=> constant (Recommended)
hello_world = 'Hello World'           #=> not constant
```



## Change value of constant
```ruby
MY_CONSTANT = 1000                    
MY_CONSTANT = 2000 #=> Modify value to 2000

warning: already initialized constant MY_CONSTANT
warning: previous definition of MY_CONSTANT was here

MY_CONSTANT       #=> After change: 2000
```

Program will show warning message when you modify value of a constant, because you should use variables if you want to change their values.

## Tips:
- Use all uppercase letter with underscore to seperate words when declaring a constant (like this NEW_CONSTANT).
- Should *NOT* change constant value.

