# TypeScript: Interface vs Type – What’s the Difference?

When you're writing code in TypeScript, you'll often need to define the **shape** of an object. There are two powerful tools for this: `interface` and `type`. While they can often be used interchangeably, they also have key differences.

In this blog, I’ll break down their similarities, differences, and when to use which.

---

##  Similarities

Both `interface` and `type` in TypeScript can:

- Describe the shape of an object
- Be extended
- Add optional and readonly properties
- Work with functions and arrays

Example using `interface`:


interface User {
  name: string;
  age: number;
}
Example using `type`:


type User = {
  name: string;
  age: number;
}

# interface supports extending other interfaces or types.
# type can use intersection (&) to achieve similar results.