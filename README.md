# Deep Copy
A lesson in `deepCopy()` for novice JavaScript programmers.

## Prerequisites

Basic understanding of JavaScript.

## Contents

- [Lecture 1. Introduction to deep copying](#lec1)

## <a name="lec1">Lecture 1. Introduction to deep copyings</a>

Recall, JavaScript uses "references."

Study the following console interaction:

<img src="foo-bar.png" width=500>

In `var b = a;`, `b` acquires `a`'s reference to the array.

`b` does not receive a duplicate array.

If you want `b` to have a duplicated array, you've got to do it the hard way:

```js
var b = new Array(a.length);
for (var i = 0; i < a.length; i++) {
  b[i] = a[i];
}
```

Study the following console interaction:

<img src="foo-bar-2.png" width=500>

That's the idea of deep copying.


