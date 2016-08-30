find() does not mutate the array on which it is called.

```js
function Car(model) {
  this.model = model;
}

var cars = [
  new Car('Buick'),
  new Car('Camaro'),
  new Car('Focus')
];

cars.find(function (car) {
  return car.model === 'Focus'
});

```
