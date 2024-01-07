🚀 TypeScript Fundamentals

## What is TypeScript?

TypeScript is a programming language developed by Microsoft that is a superset of JavaScript. 
It is designed for developing enterprise scale JavaScript applications.

## Topics

- Primitive Types
- The `any` Type
- Arrays
- Tuples
- Enums
- Functions
- Objects
- Type 

## Built-in Types

JavaScript has built-in types such as:

- Number
- String
- Boolean
- Null
- Undefined
- Object

TypeScript extends this list and introduces new types like:

- Any
- Unknown
- Never
- Enum
- Tuple

## Primitive Types

In TypeScript, primitive types include `number`, `string`, and `boolean`. You can declare and initialize variables without explicitly providing types,
as the TypeScript compiler can infer them based on the assigned values.

let sales = 123_456_789;
let course = 'TypeScript';
let is_published = true;

## The any Type

The any type in TypeScript represents any kind of value.
However, it's recommended to avoid using any as much as possible, 
as it undermines the benefits of using TypeScript's static typing.

const level: any;

## Arrays

Arrays in TypeScript can be declared with explicit type annotations:

let numbers: number[] = [1, 2, 3];

## Tuples

Tuples are fixed-length arrays where each element has a specific type. 
They are useful for working with pairs of values.

let user: [number, string] = [1, 'Azar'];

## Enums

Enums in TypeScript represent a list of related constants. 
They provide a way to define named numeric constants.

const enum Size {
  Small = 1,
  Medium,
  Large
}

let mySize = Size.Medium;

## Functions

Functions in TypeScript can have explicit parameter and return types. 
The TypeScript compiler can also infer types in many cases.

function add(a: number, b: number): number {
  return a + b;
}

## Objects 

Objects in TypeScript can represent complex structures. 
You can define an object type using interfaces or type aliases.

interface Person {
  name: string;
  age: number;
}

let person: Person = {
  name: 'John Doe',
  age: 30
};

## Type

The type keyword in TypeScript allows you to create aliases for types. 
It's particularly useful when you want to reuse complex type definitions:

type Point = {
  x: number;
  y: number;
};

let coordinates: Point = { x: 1, y: 2 };
