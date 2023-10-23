Typescript mein "Assignability Error" hota hai jab aap kisi variable ya function ko ek specific data type se assign karne ki koshish karte hain, lekin assignment ke liye data types compatible nahi hote. Chaliye ek aasan example ke sath samjhe:

**Example: Assignability Error in Variable Assignment**
```typescript
let name: string = "John Doe";
name = 42;
```

Yahan, `name` variable ko `string` data type ke sath define kiya gaya hai. Lekin phir, aapne isse `42` number se overwrite karne ki koshish ki hai. Isse "Assignability Error" aayega, kyun ki aap `string` ko `number` ke sath assign nahi kar sakte.

Sahi tarike se `name` variable ko assign karne ka tareeka:
```typescript
let name: string = "John Doe";
```

**Example: Assignability Error in Function Argument**
```typescript
function greet(message: string) {
    console.log("Message: " + message);
}

greet(42);
```

Yahan, `greet` function ko `string` type ke argument ke sath define kiya gaya hai. Lekin phir aapne function call mein `42` number pass kiya hai. Isse "Assignability Error" aayega, kyun ki function argument aur parameter ki data types match nahi kar rahi hain.

Sahi tarike se `greet` function ko call karne ka tareeka:
```typescript
greet("Hello, World");
```

Assignability errors Typescript ke type system ke hisab se data types ke assignment ke sahi aur galat tareekon ko detect karne mein madadgar hote hain. In errors ko resolve karna, code quality aur reliability ko badhata hai.