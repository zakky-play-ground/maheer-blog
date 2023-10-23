Typescript mein aam taur par istemal hone wale "everyday types" ya "primitive types" hote hain. Yahan kuch important everyday types, bullet points aur examples ke saath:

1. **String (String Type):**
   - Example: `let name: string = "John";`

2. **Number (Number Type):**
   - Example: `let age: number = 30;`

3. **Boolean (Boolean Type):**
   - Example: `let isStudent: boolean = true;`

4. **Array (Array Type):**
   - Example: `let fruits: string[] = ["apple", "banana", "cherry"];`

5. **Tuple (Tuple Type):**
   - Example: `let student: [string, number] = ["John", 25];`

6. **Object (Object Type):**
   - Example: `let person: { name: string, age: number } = { name: "John", age: 30 };`

7. **Any (Any Type):**
   - Example: `let dynamicValue: any = "Hello";`

8. **Void (Void Type):**
   - Example: `function logMessage(): void { console.log("Message"); }`

9. **Union (Union Type):**
   - Example: `let result: string | number = "Hello";`

10. **Enum (Enum Type):**
    - Example: 
    ```typescript
    enum Days {
        Sunday,
        Monday,
        Tuesday
    }
    let today: Days = Days.Monday;
    ```

Yeh everyday types TypeScript mein aam taur par istemal hote hain. In types ka istemal aap variables, functions, aur objects ke data types specify karne ke liye karte hain.



Tuples, arrays, aur objects Typescript mein data ko store karne ke alag-alag tareekon ko represent karte hain aur unme kuch khas fark hote hain:

**1. Tuple:**
   - Tuples fixed length arrays hoti hain, jisme har element ka specific data type hota hai.
   - Tuples mein elements order mein store hote hain aur unka access index ke through hota hai.
   - Example:
     ```typescript
     let person: [string, number] = ["John", 30];
     ```

**2. Array:**
   - Arrays variable length lists hote hain, jisme elements aik hi data type ke hote hain.
   - Arrays mein elements bina kisi fixed order ya sequence ke store hote hain, aur unka access index ke through hota hai.
   - Example:
     ```typescript
     let fruits: string[] = ["apple", "banana", "cherry"];
     ```

**3. Object:**
   - Objects key-value pairs ki collection hote hain, jisme values ki data type alag alag ho sakti hain.
   - Objects mein har key ke sath associated value hota hai aur unka access key ke through hota hai.
   - Example:
     ```typescript
     let person: { name: string, age: number } = { name: "John", age: 30 };
     ```

In teeno mein se har ek ka istemal specific use case ke hisab se hota hai. Tuple fixed length data structures ke liye istemal hoti hai, array variable length lists ke liye, aur object data modeling ke liye jahan key-value pairs important hain. Aap in tino types ko apne requirements ke hisab se istemal kar sakte hain.





