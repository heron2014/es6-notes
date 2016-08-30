```js
// Balance paranthesis

"()()()()" //balanced
"(((())))" //balanced

"))))" //not
"())))"
")("

function balanceParams(string) {
  return !string.split('').reduce(function(prev, char) {

    if (previous < 0) {return previous;} //case ")("
    if(char === '(') {
      return ++previous;
    }

    if(char === ')') {
      return --previous;
    }

    return previous;
  }, 0);
}

balanceParams("((((")
console.log(!0) //true
console.log(!4) //false
 ```


 Remove duplicates:

 ```js

var numbers = [1, 1, 2, 3, 4, 4];
const unique = ( array => [...new Set(array)] );

console.log('-------------------------');
function unique(array) {
    return array.reduce(function (acc, num) {
        var numInAcc = acc.find(item => item === num);

        if (!numInAcc) {
            acc.push(num);

        }

        return acc;
    }, []);
}

var numbers = [1, 1, 2, 3, 4, 4];
console.log(unique(numbers))

 ```
