# CSS transform: rotate()

## What is rotate()?

`rotate()` rotates an element clockwise or counterclockwise.

It is used with the `transform` property.

---

# 1️⃣ Basic Syntax

```css
transform: rotate(45deg);
```

Rotates element 45 degrees clockwise.

---

# 2️⃣ Units

Most common unit:

```
deg  → degrees
```

Other units (less common):

- rad (radians)
- turn (1turn = 360deg)

Example:

```css
transform: rotate(0.5turn);   /* 180deg */
```

---

# 3️⃣ Negative Rotation

```css
transform: rotate(-45deg);
```

Negative value rotates counterclockwise.

---

# 4️⃣ Rotate with Hover

```css
.box {
  transition: transform 0.3s ease;
}

.box:hover {
  transform: rotate(10deg);
}
```

Creates smooth rotation effect.

---

# 5️⃣ Transform Origin

By default, element rotates from its center.

Change origin using:

```css
transform-origin: top left;
```

Examples:

- center (default)
- top
- bottom
- left
- right
- 50% 50%

---

# 6️⃣ Multiple Transforms

```css
transform: rotate(45deg) scale(1.2) translateX(20px);
```

Transforms are applied from left to right.

---

# Important Rules

- Does NOT affect document layout
- Does NOT change element position in flow
- Can be animated with transition
- Can combine with scale, translate, skew

---

# Common Uses

- Hover tilt effect
- Rotating icons
- Loading spinners
- Decorative UI effects