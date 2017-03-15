# coolgebra-js

A cool vector & matrix math API that allows chaining and nesting of operations.
coolgebra.js is a work in progress. It is written in ES6 and may need to be transpiled for browser environments.

Vectors are represented by arrays.
<br/>[x,y,z,w]
  
Wrap the first vector in your sequence with $().
<br/>$([x,y,z])

Chain as many operators as you want.
<br/>End the sequence with .$$
<br/>$([1,1]).plus(3).times([4,5]).rotate(1,2).unit().$$
<br/>==> [-0.9019371851463437, 0.4318672412331016]

You can nest operations:
<br/>$([3,4]).plus ($([1,1]).times(3).$$) .$$

(Spaces added for clarity, delete in actual code)
as long as each nested sequence begins and ends with $() and .$$.
