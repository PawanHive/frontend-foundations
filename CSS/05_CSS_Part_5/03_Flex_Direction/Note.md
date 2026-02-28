# flex-direction in Flexbox

## What is flex-direction?

`flex-direction` controls the **main axis direction**  
inside a flex container.

It defines how flex items are placed.

---

# 1️⃣ Default Value

```css
flex-direction: row;
```

Items are arranged:

```
Left → Right
```

Main axis = horizontal  
Cross axis = vertical  

---

# 2️⃣ flex-direction Values

## 🔹 row (default)

```css
flex-direction: row;
```

Items go left to right.

---

## 🔹 row-reverse

```css
flex-direction: row-reverse;
```

Items go right to left.

---

## 🔹 column

```css
flex-direction: column;
```

Items go top to bottom.

Main axis = vertical  
Cross axis = horizontal  

---

## 🔹 column-reverse

```css
flex-direction: column-reverse;
```

Items go bottom to top.

---

# 3️⃣ Why It’s Important

`flex-direction` changes:

- Main axis
- How justify-content works
- How align-items works

Example:

If direction = row  
→ justify-content = horizontal alignment  

If direction = column  
→ justify-content = vertical alignment  

---

# 4️⃣ Example

```css
.container {
  display: flex;
  flex-direction: column;
}
```

Items stack vertically.

---

# Key Rule

Main axis depends on flex-direction.

Everything in flexbox revolves around the main axis.

---

# Quick Summary

| Value          | Direction        | Main Axis   |
|---------------|-----------------|------------|
| row           | Left → Right    | Horizontal |
| row-reverse   | Right → Left    | Horizontal |
| column        | Top → Bottom    | Vertical   |
| column-reverse| Bottom → Top    | Vertical   |
