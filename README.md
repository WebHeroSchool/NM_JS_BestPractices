# JS Best Practices
## Use expanded syntax
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

## You should include spaces between operators and operands, parameters, etc.
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
## All statements must end with semicolons (";")
> We require them in all of our code samples even though they're technically optional in JavaScript because we feel that it leads to code that is clearer and more precise about where each statement ends.

>> `BAD`:
```js
let name = 'Natasha'

```

>> GOOD:
```js
let name = 'Natasha';

```
