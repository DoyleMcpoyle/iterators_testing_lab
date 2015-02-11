##Descriptions of Iterators

###Instructions
Below you will find a list of methods. In the space provided below each, please provide a brief description of what this method does based upon your review of the Docs. 

###Array methods:
May be helpful to look in [Enumerable](http://ruby-doc.org/core-2.2.0/Enumerable.html) as well...

####select: Returns a new array containing all elements of enum for which the given block returns a true value. If no block is given, an Enumerator is returned instead. 


####reject: Returns an array for all elements of enum for which the given block returns false. I no block is given, an Enumerator is returned instead.

####map: Returns a new array with the results of running block once for every element in enum. If no block is given, an enumerator is returned instead.

####detect: Passes each entry in enum to block. Returns the first for which block is not false. If no object matches, calls ifnone and returns its result when it is specified, or returns nil otherwise.

####inject: Combines all elements of enum by applying a binary operation, specified by a block or a symbol that names a method or operator. If you specify a block, then for each element in enum the block is passed an accumulator value (memo) and the element. If you specify a symbol instead, then each element in  the collection will be passed to the named method of memo. In either case, the result becomes the new value for memo. At the end of the iteration, the final value of memo is the return value for the method. 

If you do not explicitly specify an initial value for memo, then the first element of collection is used as the initial value of memo.

####partition: Returns two arrays, the first containing the elements of enum for which the block evaluates to true, the second containing the rest. 

If no block is given, an enumerator is returned instead. 

####sort: Returns an array containing the items in enum sorted, either according to their own <=> method, or by using the results of the supplied block. The block should return -1, 0, or +1 depending on the comparison between a and b. As of Ruby 1.8, the method Enumerable#sort_by implements a built-in Schwartzian Transform, useful when key computation or comparison is expensive. 

####one?: Passes each element of the collection to the given block. The method returns true if the block returns true exactly once. If the block is not given, one? will return true only if exactly one of the collection members is true. 

####none?: Passes each element of the collection to the given block. The method returns true if the block never returns true for all elements. If the block is not given, none? will return true only if none of the collection members is true. 

####all?: Passes each element of the collection to the given block. The method returns true if the block never returns false or nil. If the block is not given, Ruby adds an implicit block of { |obj| obj } which will cause all? to return true when none of the collection members are false or nil.

####empty?: Returns true is self contains no elements.

####eql?: Returns true if self and other are the same object, or are both arrays with the same content. (according to Object#eql?)

####include?: Returns true if the given object is present in self (that is, if any element == object), otherwise returns false.

####nil?: Only the object nil responds true to nil?. 

###Hash methods:

####key?: Returns true if the given key is present in hsh. 

####keys: Returns a new array populated with the keys from this hash. See also Hash#values.

####delete: Deletes the key-value pair and returns the value from hsh whose key is equal to key. If the key is not found, returns the default value. If the optional code block is given and the key is not found, pass in the key and return the result of block. 

####delete_if: Deletes every key-value pair from hsh for which block evaluates to true. If no block is given, an enumerator is returned instead. 
