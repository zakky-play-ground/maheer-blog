Typescript mein "Type Error" ya "Type Mismatch Error" hota hai jab aap kisi variable, function, ya expression ke sath data types ke mismatch ke karan code mein error create karte hain. Typescript, static typing language hai, jisse aap data types define karke type errors se bach sakte hain. Chaliye ek simple example ke sath dekhe:

**Example: Type Error in Variable Assignment**
```typescript
let age: number = 30;
age = "thirty";
```

Yahan, pehle `age` variable ko `number` type ke sath define kiya gaya hai. Phir, `age` ko `"thirty"` string se overwrite karne ki koshish ki gayi hai. Isse "Type Error" ya "Type Mismatch Error" aayega, kyun ki aap string ko number mein assign nahi kar sakte.

Correct way to assign `age` as a number:
```typescript
let age: number = 30;
```

**Example: Type Error in Function Argument**
```typescript
function add(a: number, b: number): number {
    return a + b;
}

const result = add(5, "7");
```

Yahan, `add` function ko `number` type ke arguments ke sath define kiya gaya hai, lekin function call mein `"7"` string pass kiya gaya hai. Isse Type Error aayega, kyun ki function arguments ki data types match nahi kar rahi hain.

Correct way to call `add` function:
```typescript
const result = add(5, 7);
```

Typescript type errors aapko code likhte waqt hi pata chal jate hain aur aapko sahi data types ka use karne ki guidance dete hain. Isse aap bugs ko pehle se detect kar sakte hain aur code quality improve ho sakti hai.