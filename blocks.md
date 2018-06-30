# Blocks

## What is a block code?

- A ruby code block is code between braces **{}** or **do..end**
- Using braces **{ }** for single-line blocks
- Using **do..end** for multi-line blocks.

## Examples

```ruby
# Use braces for single line blocks
5.times { puts "Welcome to block code" }

# Use do..end for multi-line blocks
5.times do
  print "Hello "
  puts "friends"
end
```

## Variables for block

Variables for blocks are local to the block, they die when the block is executed.

```ruby
x = 10
3.times do |x|
  puts "x inside the block: #{x}"  
end
puts "x outside the block: #{x}"

# Output
x inside the block: 0
x inside the block: 1
x inside the block: 2 
x outside the block: 10  
```
