This repository refers to Day 4 of the JavaScript 30 for 30 challenge https://javascript30.com/
In todays challenge I did not so much as make a project but instead worked with several arrays using array protoypes. 
The challenge was to use the filter, map, sort, reduce methods on arrays to learn how to use them. 

What I learned: 
Array.prototype.filter()- 
this allows users to create a new array with elements that have passed a test created within the function. 
Example: 
const animals = [ 
{ name: 'Max' , type: 'dog' },
{ name: 'Spot', type: 'dog' }, 
{ name: 'whiskers', type: 'cat'}]; 
const dogs = animals.filter(animals => animals.type == 'dog')
//filtered array dogs is [ { name: 'Max', type: 'dog' }, { name: 'Spot', type: 'dog' } ] 

Array.prototype.map() - 
this allows users to create a new array with a function that is called on every element within the array. This in turn returns 
an array equal in size to the original array unlike what is seen in .filter(). 
Example: 
const numbers = [1, 2, 3, 4, 5]; 
const timesTwo = numbers.map (x => x * 2); 
This will return an array [2, 4, 6, 8, 10] 

Array.prototype.sort() - 
this allows you to sort elements in an array. By default this will sort elements in an array alphabetically and numeric but 
you can also use if statements to set sorting rules. 
When sorting numberically, numbers are sorted by Unicode code points.  
Example: 
const numbers = [1, 10, 5, 2]; 
const sorted = numbers.sort(); 
this will return [1, 10, 2, 5] as 10 is before two in Unicode code points. 

Array.prototype.reduce() - 
this allows you to reduce all the elements in an array into a single value through running a given function 
on each element in an array. 
Basic example: 
const numbers = [1, 2, 3,4]; 
const addNumbers = numbers.reduce(total, num) => total + num); 
this will return [10]
There are more advanced ways to use reduce however I did not go into them in this project. 

Ternary Operation - 
this is used in place of an if statement. The purpose of using this in this project was to write
shorter and cleaner code. ternary operations look like this:
condition ? expression 1 : expression 2 
This condition determines which expression will be returned

Array.from - 
this enables users to create an array from iterable objects or array-like objects. 
example: 
const words = 'hello';
const makeAnArray = Array.from(words); 
returns [ 'h', 'e', 'l', 'l', 'o' ]



