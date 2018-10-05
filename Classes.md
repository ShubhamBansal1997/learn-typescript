# Classes
- object oriented class approach
- quite similar to java and c#
  ```
  class Employee {
    employeeName : string,

    constructor(name: string) {
      this.employeeName = name;
    }
    greet() {
      console.log(`Good Morning ${this.employeeName}`);
    }
  }
  let emp1 = new Employee('Shubham');
  console.log(emp1.employeeName);
  emp1.greet();
  ```
- Inheritance 
  ```
  class Manager extends Employee {
    constructor(managerName: string) {
      super(managerName);
    }
    deletgateWork() {
      console.log(`Manager delegating tasks`);
    }
  }
  let m1 = new Manager('Shubham1');
  m1.deletegateWork();
  m1.greet();
  console.log(m1.employeeName);
  ```


