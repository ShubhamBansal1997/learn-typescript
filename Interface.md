# Interfaces in TypeScript

```
function fullName(person: { firstName: string, lastName: string }) {
  console.log(`${person.firstName} ${person.lastName}`);
}
let p = {
  firstName: 'Shubham',
  lastName: 'Bansal'
};
```
- The example is quite simple where the person object contains only two properties lets imagine a situation where the person object contain multiple properties. So, to avoid that situation we gonna use interface.
```
interface Person {
  firstName: string;
  lastName: string;
}

function fullName(person: Person) {
  console.log(`${person.firstName} ${person.lastName}`);
}

let p = {
  firstName: 'Shubham',
  lastName: 'Bansal'
}
```
- Easy to maintain
- Code is clean
- Change in interface is reflected everywhere
- Same Optional (?) thing work here
