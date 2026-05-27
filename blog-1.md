# Why `unknown` is Safer Than `any`

## Introduction

TypeScript provides different data types for safer coding. Two important types are `any` and `unknown`.

## What is `any`?

The `any` type disables type checking.

```ts
let data: any = "Hello";
data = 100;
TypeScript allows everything with any.

Problem with any
let value: any = 50;
value.toUpperCase();
This creates runtime errors because numbers do not have toUpperCase().

What is unknown?

unknown is safer because we must check the type first.
let value: unknown = "TypeScript";
Type Narrowing
if (typeof value === "string") {
  value.toUpperCase();
}
This process is called type narrowing.

Conclusion

unknown is safer than any because it forces developers to check types before using values.