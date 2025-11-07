# ITERATION

## While Looping

```
while(condition) {
  statements;
  increment/decrement;
}
```

**Note:** Kamu tidak dapat mendeklarasikan variabel di dalam kondisi while.

## Do...While Looping

```
do {
  statements;
  increment/decrement;
} while(condition)
```

**Note:** Statements di dalam body do tetap tereksekusi satu kali saja, walaupun kondisi while bernilai false.

## For Looping

```
for(condition, increment/decrement) {
  statements;
}
```

## Looping Control Flow

**Skip The One of Iteration:**

```
for(condition, increment/decrement) {
  if(a == b) continue;
  statements;
}
```

**Skip The More of Iteration:**

```
for(condition, increment/decrement) {
  if(a > b && a < b) continue;
  statements;
}
```

**Stop The Next of Iteration:**

```
for(condition, increment/decrement) {
  if(a == b) break;
  statements;
}
```