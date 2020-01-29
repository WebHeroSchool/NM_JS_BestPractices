# JS Best Practices
## 1. Use expanded syntax
> This maximizes readability
>> `BAD`:
```js
function myFunc() { console.log('Hello!'); }
```
>> GOOD
```js
function myFunc() {
  console.log('Hello!');
}
```

## 2. You should include spaces between operators and operands, parameters, etc.

> Code will be more readable


>> `BAD`:

```js
if(dayOfWeek===7&&weather==='sunny'){
  goOnTrip('beach','car',['ice cream','bucket and spade','beach towel']);
}
```

>> GOOD:
```js
if(dayOfWeek === 7 && weather === 'sunny') {
  goOnTrip('beach', 'car', ['ice cream', 'bucket and spade', 'beach towel']);
}
```
## 3. All statements must end with semicolons (";")
> We require them in all of our code samples even though they're technically optional in JavaScript because we feel that it leads to code that is clearer and more precise about where each statement ends.

>> `BAD`:
```js
let name = 'Natasha'

```

>> GOOD:
```js
let name = 'Natasha';

```
## 4. Don't include padding spaces after opening brackets or before closing brackets — (myVar), not ( myVar ). 
      
  >> `BAD`:
  ```js
  function sum( num1, num2 ){}
  
  ```
  
  >> GOOD:
  ```js
  function sum(num1, num2){}
 ``` 
    
## 5. There should be no space between a control statement keyword, function, or loop keyword and its opening parenthesis (e.g. if() { ... }, function myFunc() { ... }, for(...) { ... }).
## There should be a space between the parentheses and the opening curly brace


 >>  `BAD`:

```js
    function sum (num1, num2){}
```
    >> GOOD:
  ```js
    function sum(num1, num2) {}
   ```    

## 6. Use single quotes in JavaScript, wherever single quotes are needed in syntax.

>>  `BAD`:
```js
    let str = "string";
```
    >> GOOD:
  ```js
    let str = 'string';
   ``` 
## 7. For variable names use lowerCamelCasing, and use concise, human-readable, semantic names where appropriate.
   >>  `BAD`:
```js
    let thisIsaveryLONGVariableThatRecordsPlayerscore345654 = 0;
    let s = d/t;
```
  >> GOOD:
  ```js
    let playerScore = 0;
    let speed = distance / time;
   ``` 
## 8. When inserting strings into DOM nodes, use Node.textContent not innerHTML
> Because textContent is a lot more efficient, and less error-prone than innerHTML.

 >>  `BAD`: 
```js
    let text = 'Hello to all you good people';
    const para = document.createElement('p');
    para.innerHTML = text;
   
```

  >> GOOD:
  ```js
    let text = 'Hello to all you good people';
    const para = document.createElement('p');
    para.textContent = text;
```

## 9. 