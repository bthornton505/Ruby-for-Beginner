# `.sub` and `.gsub` in ruby

Both methods are for replacing part of a string.

### `.sub`

`String#sub` method allows to replace first occurrence of pattern to another substring.

```ruby
"some string with spaces".sub(" ", "_") # => "some_string with spaces"
```

### `.gsub`

`String#gsub` method allows to replace all occurrences of pattern to another substring.

```ruby
"some string with spaces".sub(" ", "_") # => "some_string_with_spaces"
```

### Additional info

Both `.sub` and `.gsub` methods create a new string. So if you have a variable

```ruby
my_string = "my string with spaces"
my_string.sub("my string", "new string") # => "new string with spaces"
my_string # => "my string with spaces"
```

If you want to transform string in place, you can add `!` character to those methods (resulting in `.sub!` & `.gsub!`)
```ruby
my_string = "my string with spaces"
my_string.sub!("my string", "new string") # => "new string with spaces"
my_string # => "new string with spaces"
```
