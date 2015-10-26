### Operating on Arrays
There are a number of other methods available for manipulating arrays. You can learn more about them [here](http://ruby-doc.org/core-2.2.0/Array.html), but we'll look at just a few examples together.
#### The `.sort` Method
This method rearranges the contents of the array by, well, sorting them. For strings, this means alphabetically, for numerical values, this means from smallest number to highest number.
**Advanced:** ​*The*​ `.sort` ​*method works by implicitly comparing elements with the "spaceship" operator*​ `<=>` ​*(because it looks like a flying saucer, swoosh!) and moving them accordingly.*​
```ruby
famous_cats = ["lil' bub", "grumpy cat", "Maru"]
famous_cats.sort
  => ["grumpy cat", "lil' bub", "Maru"]
```
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
Add Comment
Class : Array - Ruby 2.2.0

sophie [2:17 PM]
also .first, .last and .size
