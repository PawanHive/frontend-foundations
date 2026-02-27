# CSS transform: translate()

## What is translate()?

`translate()` moves an element from its original position.

It is used with the `transform` property.

---

# 1️⃣ Basic Syntax

```css
transform: translate(20px, 10px);
```

First value → move horizontally (X axis)  
Second value → move vertically (Y axis)

---

# 2️⃣ Single Value

```css
transform: translate(20px);
```

Moves only on X axis.

---

# 3️⃣ Translate X and Y Separately

```css
transform: translateX(30px);
transform: translateY(50px);
```

---

# 4️⃣ Using Percentage

```css
transform: translate(50%, 50%);
```

Percentage is based on the element’s own size  
(not parent size).

---

# 5️⃣ Negative Values

```css
transform: translate(-20px, -10px);
```

Moves left and up.

---

# 6️⃣ Translate with Hover

```css
.box {
  transition: transform 0.3s ease;
}

.box:hover {
  transform: translateY(-5px);
}
```

Creates lift effect.

---

# 7️⃣ Important Rules

- Does NOT affect document layout
- Other elements do not move
- Element keeps its original space
- Works well with transition

---

# 8️⃣ Centering Trick (Common)

```css
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
```

Used to perfectly center an element.

---

# Common Uses

- Hover lift effects
- Slide animations
- Centering elements
- UI micro-interactions