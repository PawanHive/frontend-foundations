# CSS transform: scale()

## What is scale()?

`scale()` changes the size of an element.

It is used with the `transform` property.

---

# 1️⃣ Basic Syntax

```css
transform: scale(1.2);
```

1.2 = 120% of original size  
1 = original size  
0.5 = 50% size  

---

# 2️⃣ Scale X and Y Separately

```css
transform: scale(1.5, 0.8);
```

First value → width (X axis)  
Second value → height (Y axis)

---

# 3️⃣ Scale Only One Direction

```css
transform: scaleX(1.5);
transform: scaleY(0.8);
```

---

# 4️⃣ Scale with Hover (Common Use)

```css
.card {
  transition: transform 0.3s ease;
}

.card:hover {
  transform: scale(1.05);
}
```

Creates zoom effect.

---

# 5️⃣ Important Rules

- Does NOT affect layout flow
- Other elements do not move
- Element scales from its center (default)
- Can change origin using:

```css
transform-origin: top left;
```

---

# 6️⃣ Negative Scale

```css
transform: scale(-1);
```

Flips element horizontally.

---

# 7️⃣ Combine with Other Transforms

```css
transform: scale(1.1) rotate(5deg);
```

Transforms apply left to right.

---

# Common Uses

- Hover zoom effects
- Button press animation
- Image zoom
- Card lift effects
- UI micro-interactions