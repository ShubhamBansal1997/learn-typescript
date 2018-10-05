# Variable Types
- Important feature of Typescript
- Variable types in TypeScript
  + Boolean
  + String
  + Number
- Example
  ```
  let isBegineer: boolean = true;
  let total: number = 0;
  let name: string = 'Shubham';

  let myself: string = `My name is ${name}
  Started in the typscript`;
  // multiple lines in embedded expressions
  ```
- Benefits of Variable Types
  + Static type checking
  + Accurate Intelligence
- null and undefined types
  + sub types of classified types
  + Example
  ```
  let n: null = null;
  let u: undefined = undefined;
  ```
- array types
  + Single type
   ```
   let test: number[] = [1,2,3];
   let test2: Array<number> = [1,2,3];
   ```
  + Tuple Type
    ```
    let test: [string, number] = ['Shubham', 22];
    // same order and same type
    ```
- enum type
  ```
  enum Colors { Red, Orange, Green };
  let c: Color = Colors.Green;
  conosle.log(c);
  // 1
  enum Colors { Red = 5, Orange = 4, Green = 3 };
  let c: Color = Colors.Red;
  console.log(c);
  // 5
- any type
  + Most Capable type
  + For Dynamic values
  + Can be assigned to any type
  + Example
  ```
  let test: any = 10;
  test = 'Test';
  test = true;
  test()
  test.toUpperCase();
  test.name;
  ```
- unkown type
  + Introducted in 3.0
  + similar to any type
  + any type can be assigned to unkown type
  + But you can't access the property of any type just like you did in any type
  ```
  let test: unknown = 10;
  (test as string).toUpperCase();
  // type assertion
  ```
- user defined type guard
  ```
  let test: unkown = 10;
  function hasName(obj: any ): obj is { name: string } {
    return !!obj &&
      typeof obj === "object" &&
      "name" in obj
  }
  if (hasName(myVariable)) {
      console.log(myVariable.name);
  }
  ```

## Type Inference

```
// in js
let a;
a = 10;
a = true;

// in ts
let b = 20;
b = true;
// show warning
// type intelligence
```
- multitype
  ```
  let multitype: number | boolean;
  multitype = 20;
  multitype = true;
  ```


