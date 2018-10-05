# Access Modifiers
- Access Modifiers are basically keywords that set the accessability of the properties and methods in the class
- Public
- Private
- Protected
- By default every member is public, just like in our last example

# Private
If the access modifier is private then we can be accessed within the class only
- way to secure the member
- cannot access in the derived class too
```
class Employee {
  private employeeName: string;
  ....
}

...
conosole.log(emp1.employeeName);
// this statement throws error
...
```

# Protected
If we want to access in the derived class but not outside the class then the protected access modifier comes into the play.



