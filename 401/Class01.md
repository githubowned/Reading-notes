# Readings: Node Ecosystem, TDD, CI/CD
1. Describe (in plain English) what Array.map() does

- The map() method creates a new array with the results of calling a function for every array element.

- The map() method calls the provided function once for each element in an array, in order.

<p>&nbsp;</p>

> Note: map() does not execute the function for array elements without values.

> Note: this method does not change the original array.

<p>&nbsp;</p>


```js
let numbers = [1, 4, 9]
let roots = numbers.map(function(num) {
    return Math.sqrt(num)
})
```

<p>&nbsp;</p>
<p>&nbsp;</p>





2. Describe (in plain English) what Array.reduce() does

- he reduce() method reduces the array to a single value.

- The reduce() method executes a provided function for each value of the array (from left-to-right).

- The return value of the function is stored in an accumulator (result/total).

> Note: reduce() does not execute the function for array elements without values.

> Note: This method does not change the original array.

```js
const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// expected output: 15
```
<p>&nbsp;</p>
<p>&nbsp;</p>

3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
With normal Promise .then() syntax
Again with async / await syntax

<p>&nbsp;</p>


```js
try {
  const res = await request
    .get('http+unix://%2Fabsolute%2Fpath%2Fto%2Funix.sock/search');
 
} catch(err) {
  // err.message, err.response
}
``` 
<p>&nbsp;</p>


```js
  superagent.get(`https://swapi.dev/api/people`).then(data=>{
      data.body.results.forEach(item=>{
   console.log({[item.name] : item.url})
     })
  }).catch(error=>console.log(error));
  ```
  <p>&nbsp;</p>


```js
try
{ let data=await superagent.get(`https://geocode.xyz/${city}?json=1`);
 console.log(city,data.body.longt,data.body.latt)
  }

 catch(error){
     console.log(error)
     }
```
<p>&nbsp;</p>
<p>&nbsp;</p>


4. Explain promises as though you were mentoring a Code 301 level student

- A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.

<p>&nbsp;</p>


- A Promise is in one of these states:

1. pending: initial state, neither fulfilled nor rejected.
2. fulfilled: meaning that the operation was completed successfully.
3. rejected: meaning that the operation failed.




