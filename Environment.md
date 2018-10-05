# Environment Setup
- Install the latest nodejs stable relase on your OS from [https://nodejs.org/](https://nodejs.org/)
- Install typescript
 ```
 npm install -g typescript
 ```

## Writing Hello World Program
- Create a file name main.ts
- Write in the file
  ```
  let message = 'Hello World';
  conosle.log(message);
  ```
- Compile the file using terminal
  ```
  >>> tsc main.ts
  ```
- A main.js file is generated
  ```
  var message = 'Hello World';
  console.log(message);
  ```
- Run using node
  ```
  >>> node main.js
  ```
- See the Output
  ```
  Hello World
  ```


# File is treated is as script not a module which means it shares global scope
- Export nothing
   ```
   export {}
   ```
- After recompilling js file would be
  ```
  "use strict";
  exports.__esModule = true;
  var message = "Hello World";
  console.log(message);
  ```

# Implmenting watchman
```
>>> tsc main.ts --watch
```
