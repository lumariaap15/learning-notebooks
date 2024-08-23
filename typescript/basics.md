
# TYPESCRIPT

Is Known as "a superset of javascript"
But it doesn't give you more JS features, just helps you write more accurate JS

- Recommended for large projects
- Is all about Type Safety
- STATIC CHECKING: This is a feature that languages like Java have. But in Javascript,  you can only get error feedback on execution. Typescript gives you hints on what might be wrong in static checking.
- Typescript is a development tool. Is not a lang itself. Is still converted to JavaScript.

> To compile this file into JS, run the following command:
> tsc "filename" 
```ts
//number

let userId: number = 334455.3;

//boolean

let isLoggedIn: boolean = true;
```

## REDUNDANT TYPE ASSIGNMENT

TS can automatically infer the types in this cases
```ts
let userId2 = 334455.3;

userId2 = 'hello';
```

## ANY

- this is automatically inferred when typescript does not know what to expect from the variable
- any basically disables type-checking for the variable
- to prevent typescript from asigning any, use the ***notImplicitAny*** flag
```ts
let anyValue;

function getValue(){
return true;
}

anyValue = getValue();
```

## FUNCTIONS

- Default values for params
- Return values
- Void return values
```ts
let loginUser = (name: string, age: number = 10) => {}
loginUser("Luisa")

// return values for functions
function addTwo(num: number): number{
return num + 2;
}

// return void values for functions
function consoleSomething(): void {
console.log("Hello");
}
```

# OBJECTS

Return objects in functions
```ts
function createCourse():{name: string, price: number}{
    return {name: "course", price: 399}
}
```
