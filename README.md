# Ruby Cheatsheet

A collection of code snippets that are worth reviewing. Currently going through [Learn Ruby the Hard Way](http://learnrubythehardway.org)

```
puts "#{variable_name}"
puts "%{var_001}, %{var_002}" % {var_001: 'apple', var_002: 'banana ice cream'}"
```

```
# This receives input (typically from $stdin)
gets

# This chops off newline at end
gets.chomp

# This converts string to int
gets.chomp.to_i

# Converts string to float
gets.chomp.to_f

first, second, third = ARGV
first = ARGV.first

def my_new_function(**args)
  arg1, arg2 = args
end
```

```
txt = open('my_file.txt')
puts txt.read

# Automatically truncates file to zero length
txt = open('my_file.txt', 'w')

# Manual truncate
txt.truncate(0)

# Go to position
txt.seek(0)

txt.write("hi world")
txt.close

File.exists?('file_name.txt')
```

[More options for opening files.](http://stackoverflow.com/questions/3682359/what-are-the-ruby-file-open-modes-and-options)

```
# heredoc
a = <<END
Heredocs allow multiline
strings
END
```

```
module MyModule
  def MyModule.say_hello_to(name)
    puts "Hi " + name
  end
end
```

```
string.split(' ')
list.sort
list.shift
list.pop
```

```
if 10 == 11
  puts "ten equals eleven"
elsif 11 == 11
  puts "why would you not include the last e in else???"
else
  puts "who knows.."
end
```
