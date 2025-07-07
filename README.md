# TypeScript: Interface vs Type – What is the Difference?

When you're writing code in TypeScript, we'll often need to define the **shape** of an object. There are two powerful tools for this: `interface` and `type`.They also have key differences and method.

In this blog, I’ll break down their similarities, differences.

---

## Both `interface` and `type` in TypeScript can:

- Describe the shape of an object
- They can make shape of array of object
- Be extended
- Add optional and readonly properties
- Work with functions and arrays

Example using `interface`:
interface User {
  name: string;
  age: number;
}
`Interface`supports extending other interfaces.Even not only interfaces but also Interface can extending types.It is shape very read able.I thank that every programmer understand properly this method.

Example using `type`:
type User = {
  name: string;
  age: number;
}

`Type`can use intersection `(&)` to achieve similar results.There are many types able in this tools.Among them `union` type and `intersection `type very use able,Even when you need difference type text data,You can use union type But User can take one section For example `type choseOnePerson='Tmanna'|'Halima'|'Rakib'`.Intersection is not optional Such as `type Name={name:string},type Age ={age:number}`.If we need intersection that time we have to make `type Person= Name & Age`.After that Use Person type We will be bound to give two variable data `Name and Age`,due to it is intersection.

