Topic:
`Generics`

```md id="a0y9ui"
# How Generics Make Code Reusable

## Introduction

Generics help developers create reusable and type-safe code in TypeScript.

## Generic Function Example

```ts
function identity<T>(value: T): T {
  return value;
}

Here, T represents a type.

Using Different Types
identity<string>("Hello");
identity<number>(10);

The same function works for multiple data types.

Benefits of Generics
Reusable code
Better type safety
Less duplicate code
Real Example
function getProperty<T, K extends keyof T>(obj: T, key: K): T[K] {
  return obj[key];
}

This ensures only valid object keys are used.

Conclusion

Generics help build flexible, reusable, and safe TypeScript applications.