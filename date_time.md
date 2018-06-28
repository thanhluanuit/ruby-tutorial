## Time

Time is an abstraction of dates and times. 

Examples

### Getting current time

```ruby
# Get current time using timezone of local system
Time.now  # => 2018-06-27 20:28:27 +0700

# Get current time using timezone of UTC
Time.now.utc
```

### Getting components of a Time 

```ruby
time = Time.new   # => 2018-06-27 20:32:37 +0700

time.year         # => 2018 - Year of the date 
time.month        # => 06   - Month of the date (1 to 12)
time.day          # => 27   - Day of the date (1 to 31 )

time.hour         # => 20   - 24-hour clock
time.min          # => 32
time.sec          # => 37

time.wday         # => 3    - Day of week: 0 is Sunday
time.yday         # => 178  - Day of year (365)
time.zone         # => +07  - "UTC": timezone name
```

- Get all components of a time in a array with below format:

```ruby
[sec, min, hour, day, month, year, wday, yday, isdst, zone]
```

```ruby
time = Time.new
time.to_a
=> [21, 39, 20, 27, 6, 2018, 3, 178, false, "+07"]
```

### Format a time with *strftime* 

*strftime* is a common method would use to convert time to string.

```ruby
Time.now.strftime("%B %e, %Y at %I:%M %p")
=> "June 27, 2018 at 08:48 PM"
```

### Create a time object

##### Format
```markdown
Time.new(year, month, day, hour, min, sec, utc_offset)
```

##### Examples
```ruby 
Time.new(2018, 6, 27)          #=> 2018-06-27 00:00:00 +0700 ~ Midnight 27 June 2018
Time.new(2018, 6, 27, 20, 55)  #=> 2018-06-27 20:55:00 +0700 ~ 20:55 on 27 June 2018
```
