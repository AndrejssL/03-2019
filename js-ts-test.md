## How to add question?

Question body goes here...

a) first choice  
b*) second choice (correct answer is marked with a star)  
c) third choice  
d) fourth choice  

---

## Up & Going @You Don't Know JS

```javascript
function foo(a) {
  console.log( a + b );
  let b = a;
}
foo( 2 );
```

What is the output?

a) 4  
b*) NaN  
c) 2  
d) Error  

#

How would you execute (call) this function?

```javascript
(function foo(){
  console.log( "Hello!" );
})();
```

a) This type of function expression syntax is not valid in JavaScript  
b) By calling it with foo();  
c*) No need to call it, it is immediately invoked by () at the end of the expression  
d) By calling it with foo.call();  

---

## Scope @ Closures @You Don't Know JS

```javascript
function foo() {
  const a = 4;
  console.log( this.a );
}
var a = {
  a: 2
};
var b = {
  a:a,
  foo:foo,
  b: 'hello'
}
foo.call( b );
```

What is the output?

a*) {a:2}  
b) hello  
c) 2  
d) 4  

#

Which of the following statemenets are false?

a) A block (identified by a pair of curly braces) does not define a new scope for _let_ and _const_, but it does for _var_  
b) A variable defined as _const_ or _let_ is also visible outside that block where it resides  
c) A variable defined as _var_ inside a function is visible in every part of program  
d*) All of the above  

---

## this & Object Prototypes @You Don't Know JS

Which of these is correct type assertion syntax?

a*) <string>someValue  
b*) someValue as string  
c)both  
d)none of these  

#

What does the following code print to the console?

```javascript
var object = {
  foo: function() { return (this === object); }
}
console.log(object.foo());
```

a*) true  
b) false  
c) undefined  
d) ReferenceError: this is not defined  

---

## Handbook @typescriptlang.org

```typescript
function buildName(firstName: string, lastName?: string) {
    if (lastName)
        return firstName + " " + lastName;
    else
        return firstName;
}
```

Which is the correct function call?

a*) let result1 = buildName("Bob");  
b)  let result2 = buildName("Bob", "Adams", "Sr.");  
c*) const result3 = buildName("Bob", "Adams");  
d*) var result4 = buildName("Bob");  

#

```typescript
function buildName(firstName = "Will", lastName: string) {
    return firstName + " " + lastName;
}
```

Which function call would not result in error?

a) let result1 = buildName("Bob");  
b) let result2 = buildName("Bob", "Adams", "Sr.");  
c*) let result3 = buildName("Bob", "Adams");  
d*) let result4 = buildName(undefined, "Adams");  