# CSS transform: skew()

## What is skew()?

`skew()` tilts an element along the X or Y axis.

It is used with the `transform` property.

---

# 1️⃣ Basic Syntax

```css
transform: skew(20deg, 10deg);
```

First value → skew on X axis  
Second value → skew on Y axis  

---

# 2️⃣ Skew Only One Direction

```css
transform: skewX(20deg);
transform: skewY(15deg);
```

---

# 3️⃣ Units

Most common unit:

```
deg → degrees
```

Example:

```css
transform: skew(45deg);
```

---

# 4️⃣ Skew with Hover

```css
.box {
  transition: transform 0.3s ease;
}

.box:hover {
  transform: skew(10deg);
}
```

Creates tilt effect.

---

# 5️⃣ Important Rules

- Does NOT affect document layout
- Element keeps its original space
- Can distort text inside element
- Can combine with rotate, scale, translate

---

# 6️⃣ Combine with Other Transforms

```css
transform: skew(10deg) rotate(5deg) scale(1.1);
```

Transforms apply from left to right.

---

# Common Uses

- Creative card effects
- Stylized buttons
- Angled sections
- Decorative UI elements