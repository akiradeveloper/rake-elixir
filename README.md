# Rake-Elixir

This is an implementation of Rake rewritten in Elixir.

## Elixir

Elixir is a Ruby-like new language running on Erlang VM
which puts more focuses on meta-programming to build a DSL.
This project is an experiment to examine the extensibility.

## Why not Mix but Rake clone?

Rake is my favorite tool and I want to write tasks as in Rakefile
with Elixir language. Also, I want more Ruby programmers join 
Elixir community.

## Features

This project will possibly support these rudimentary features.
At this point, I am not sure I could do this in Elixir.

```
desc "do task1"
task("task1") do 
end

desc "do task 2"
task "task2", ["task1"] do
end

desc "Let's clean up" 
task "clean"  do
end
```

To list the tasks registered

```
$ potion -T
task1 - do task 1
task2 - do task 2
clean - Let's clean up
```

To run a task

```
$ potion task1
```

## Developer

Akira Hayakawa (ruby.wktk@gmail.com)
