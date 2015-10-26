#Array Methods

###Overview
This lesson will give a deeper dive on why arrays are valuable and some useful methods you can use when working with arrays.

###Objectives
1. Sort arrays with the sort method
2. Find the first and last methods with their respective methods
3. Learn about the size of the array
4. Find if an element is in the array with the include? method
5. Understand why arrays are valuable

### Working With Arrays

#### The `.sort` Method
This method rearranges the contents of the array by, well, sorting them. For strings, this means alphabetically, for numerical values, this means from smallest number to highest number.

**Advanced:** ​*The*​ `.sort` ​*method works by implicitly comparing elements with the "spaceship" operator*​ `<=>` ​*(because it looks like a flying saucer, swoosh!) and moving them accordingly.*​

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.sort
  => ["grumpy cat", "lil' bub", "Maru"]
```
One thing to be aware of is that the return value of `famous_cats` remains unchanged after using the `sort` method on it. Meaning if you call `famous_cats` again after the sort, it will still return `["lil' bub", "grumpy cat", "Maru"]`, not the previously sorted array.

#### The `.reverse` Method
This method reverses an array.
```ruby  
famous_wizards = ["Dumbledore", "Gandalf", "Merlin"]
famous_wizards.reverse
  => ["Merlin", "Gandalf", "Dumbledore"]
```
#### The `.include?()` Method
This method will return a boolean of whether or not the array contains (or ​*includes*​) the element submitted to it inside the parentheses:

```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.include?("Garfield")
  => false
famous_cats.include?("Maru")
  => true
```
Since we are just returning `true` or `false`, the return value remains unchanged.

#### The `.first` Method

#### The `.last` Method

#### The `.size` Method
