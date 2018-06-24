# Strings

## Examples:
```ruby
'This is a string in single quote'
"This is a string in double quote"
```

## What is a String in Ruby?
String is a text with single-quote(' ') or double-quote(" ") . 

## Interpolation
Interpolation allows a string includes Ruby expression

Using:
```
"#{expression}"
```

Examples:

```ruby
ruby = "Ruby Programming"
"Welcome to #{ruby}" #=> "Welcome to Ruby Programming"

sum = 1 + 2
"Sum = #{sum}"       #=> "Sum = 3"

"1 + 2 = {1 + 2}"    #=> "1 + 2 = 3"
```

## Indexing
```ruby
string_ruby = "Welcome to String in Ruby"
```
- Get first character in string_ruby: 
    ```ruby
    irb:001> string_ruby[0]
    => "W"
    ```

- Get last character in string_ruby:  
    ```ruby
    irb:001> string_ruby[-1]
    => "y"
    ```
- Get second last character:
    ```ruby
    irb:001> string_ruby[-2]
    => "b"
    ```
 
- Get first 7 characters: 
    ```ruby
    irb:001> string_ruby[0..6]
    => "Welcome"
    ```

- Get last 4 characters: 
    ```ruby
    irb:001> string_ruby[-4..-1]
    => "Ruby"
    ```

## Common Methods in String

- Upcase a string

    ```ruby
    irb:001> "hello world".upcase     
    => "HELLO WORLD"
    ```

- Downcase a string

    ```ruby
    irb:001> "HELLO WORLD".downcase   
    => "hello world"
    ```

- Reverse characters in a string

    ```ruby
    irb:001> "hello world".reverse    
    => "dlrow olleh"
    ```

- Capitalize first character in a string

    ```ruby
    irb:001> "hello world".capitalize 
    => "Hello world"
    ```

- Get length of a string
 
    ```ruby
    irb:001> "hello world".length     
    => 11
    ```
   
- Replace a character in string by a new character

    ```ruby
    irb:001> "hello world".gsub("l", "L") 
    => "heLLo worLd"
    ```
