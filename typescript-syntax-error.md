Typescript mein syntax error ka matlab hota hai ki aapne code likhte waqt Typescript ke syntax rules ko follow nahi kiya. Typescript ek strongly typed language hai, isliye syntax errors ko resolve karna important hai. Chaliye ek simple example ke sath dekhe:

**Example 1: Syntax Error in Variable Declaration**
```typescript
let message: string = "Hello, World"
```
In this example, there is a syntax error. The correct syntax should include a semicolon `;` at the end of the line to terminate the statement:

```typescript
let message: string = "Hello, World";
```

**Example 2: Syntax Error in Function Declaration**
```typescript
function greet(name: string) {
    console.log("Hello, " name);
}
```
Here, there is a syntax error in the `console.log` line. To concatenate the `name` variable, you should use `+`:

```typescript
function greet(name: string) {
    console.log("Hello, " + name);
}
```

Typescript's compiler will highlight these syntax errors, making it easier to spot and correct them. These errors prevent your code from running correctly, so it's crucial to pay attention to the syntax rules when writing TypeScript code.