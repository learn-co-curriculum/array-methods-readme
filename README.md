# Array Methods

## Overview

This lesson will present some useful methods you can use when working with arrays.

## Objectives

1. Sort arrays with the sort method

2. Find the first and last elements of an array

3. Find the size of an array

4. Find if an element is in the array with the include? method

## Working With Arrays

### The `.sort` Method

This method rearranges the contents of the array by sorting them. For strings,
this means alphabetically, for numerical values, this means from smallest number
to highest number.

**Advanced:** ​*The*​ `.sort` ​*method works by implicitly comparing elements
with the "spaceship" operator*​ `<=>` ​*(because it looks like a flying saucer,
swoosh!) and moving them accordingly.*​

```ruby
famous_cats = ["lil' bub", "grumpy cat", "maru"]
famous_cats.sort
  => ["grumpy cat", "lil' bub", "maru"]
```

One thing to be aware of is that the return value of `famous_cats` remains
unchanged after using the `sort` method on it. Meaning if you call `famous_cats`
again after the sort, it will still return `["lil' bub", "grumpy cat", "maru"]`,
not the previously sorted array.

Because `sort` returns a new array, we generally store it into another variable.
So we would do `sorted_cats = famous_cats.sort`. Now we have two copies of the
array. One unsorted (`famous_cats`) and one sorted (`sorted_cats`). If you don't
care about the unsorted version of the array you can call `sort!`. This will
sort the existing array without requiring you to save the return into a new
variable. You'll notice the `!`. It's a ruby convention that a method with the
`!` will do the operation in place. It will modify the receiver of the method
(AKA the thing to the left of the dot).

### The `.reverse` Method

This method reverses an array.

```ruby  
famous_wizards = ["Dumbledore", "Gandalf", "Merlin"]
famous_wizards.reverse
  => ["Merlin", "Gandalf", "Dumbledore"]
```

Similarly to `sort!`, you can call `reverse!`, again modifying the receiver of
the method in place.

### The `.include?` Method

This method will return a boolean of whether or not the array contains (or
​*includes*​) the element submitted to it inside the parentheses:

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.include?("Garfield")
  => false
famous_cats.include?("Maru")
  => true
```

Since we are just returning `true` or `false`, the receiver of the method,
`famous_cats`, remains unchanged.

### The `.first` Method

This method will return the first element of the array, as its name suggests.
Again, it does not change the return value of the original array.

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.first
  => "lil' bub"
```

### The `.last` Method

This method will return the last element of the array, as its name suggests.
Again, it does not change the original array.

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.last
  => "Maru"
```

### The `.size` Method

This method will return the number of elements in the array.

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.size
  => 3
```

Even though arrays start with a 0 `index`, this method returns the actual number
of elements, starting from 1.

**Note**: Be aware that all of the methods we have covered in this reading are
case sensitive. For example, `reverse` not `Reverse`.
