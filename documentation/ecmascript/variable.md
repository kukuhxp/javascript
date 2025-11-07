# VARIABLE

## Declaration 

**Unassigned:** `let variable;`

**Assigning:** `variable = value`

**Assigned:** `let variable = value`

## Scope

```
global variable
{
  lexical variable
}
```

## Constant

**Constant Variable:**

```
const a = 8;");
a = 10; // Error
```

**Constant Array:**

```
const b = [10, 9];
b = [2, 5]; // Error
```
**Constant Object:**

```
const c = {age: 20};
c = {age: 23}; // Error
```

## Boxing & Unboxing

**Primitive Type:**

```
variable = value;
variable.method(); // Auto-boxing
```

**Non-primitive Type:**

```
variable = new Object(value); // Manual boxing
variable = Object.method(); // Unboxing
```

## Casting

- **Implicit Casting:** Casting yang dilakukan secara otomatis tanpa menggunakan method apapun.
- **Explicit Casting:** Casting yang dilakukan secara manual dengan menggunakan method.