# Function in TypeScript

## Basic Function
```
// in js
function add(a, b) {
  return a + b;
}
// in ts
function add(a: number, b: number): number {
  return a + b;
}
add(5, 10);
add(5, '12'); // error thrown here
```
- In ts all parameters are considered as the required parameters
- Optional Parameters
 ```
 function add(num1 : number, num2?: number) : number {
  if(num2) {
    return num1 + num2;
  } else {
    return num1;
  }
}
  add(5, 10);
  add(5);
  ```
  + We can add any number of optional parameter we want, just add the ?
- Default Parmeters
  ```
  function add(num1: number, num2: number = 10) : number {
    return num1 + num2;
  }
  ```
  + Default Parameters are like optional parameters with default values.
