# flex (Shorthand Property)

## What is flex?

`flex` is a shorthand property for:

- flex-grow
- flex-shrink
- flex-basis

Instead of writing 3 lines,
you can write everything in one line.

---

# 1️⃣ Full Syntax

```css
flex: grow shrink basis;
```

Example:

```css
flex: 1 1 200px;
```

Means:

```css
flex-grow: 1;
flex-shrink: 1;
flex-basis: 200px;
```

---

# 2️⃣ Understanding Each Value

## 🔹 flex-grow

How much item grows when extra space is available.

---

## 🔹 flex-shrink

How much item shrinks when space is limited.

---

## 🔹 flex-basis

Initial size before grow/shrink happens.

Works on main axis.

---

# 3️⃣ Common Shortcut Values

## 🔹 flex: 1;

```css
flex: 1;
```

Means:

```css
flex: 1 1 0%;
```

👉 All items take equal space.

Very commonly used.

---

## 🔹 flex: auto;

```css
flex: auto;
```

Means:

```css
flex: 1 1 auto;
```

Item grows and shrinks based on content size.

---

## 🔹 flex: none;

```css
flex: none;
```

Means:

```css
flex: 0 0 auto;
```

Item:
- Does NOT grow
- Does NOT shrink

---

## 🔹 flex: 0;

```css
flex: 0;
```

Means:

```css
flex: 0 1 0%;
```

---

# 4️⃣ Important Rule

If you give only one number:

```css
flex: 2;
```

It means:

```css
flex: 2 1 0%;
```

---

# 5️⃣ When To Use flex Shorthand

Use it when:

- You want clean code
- You want equal spacing
- You are building responsive layouts

---

# Quick Summary

| Value        | Meaning |
|-------------|---------|
| flex: 1     | Equal flexible space |
| flex: auto  | Flexible based on content |
| flex: none  | Fixed size |
| flex: 1 1 200px | Grow, shrink, start at 200px |