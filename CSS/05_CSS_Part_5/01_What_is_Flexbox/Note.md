# What is Flexbox?

Flexbox (Flexible Box Layout) is a **1-dimensional layout system** in CSS.

It is used to align and distribute space between items inside a container.

---

# 1️⃣ Activate Flexbox

```css
.container {
  display: flex;
}
```

This makes the element a **flex container**.

All direct children become **flex items**.

---

# 2️⃣ Main Concepts

Flexbox works on two axes:

- Main Axis (default: horizontal)
- Cross Axis (vertical)

Default direction:

```
Left → Right
```

---

# 3️⃣ Important Container Properties

## 🔹 flex-direction

```css
flex-direction: row;
```

Values:
- row (default)
- column
- row-reverse
- column-reverse

---

## 🔹 justify-content

Controls alignment on **main axis**.

```css
justify-content: center;
```

Common values:
- flex-start
- center
- flex-end
- space-between
- space-around
- space-evenly

---

## 🔹 align-items

Controls alignment on **cross axis**.

```css
align-items: center;
```

---

## 🔹 flex-wrap

```css
flex-wrap: wrap;
```

Allows items to move to next line.

---

## 🔹 gap

```css
gap: 20px;
```

Adds space between flex items.

---

# 4️⃣ Important Flex Item Properties

## 🔹 flex-grow

```css
flex-grow: 1;
```

Item can grow to fill space.

---

## 🔹 flex-shrink

Controls shrinking behavior.

---

## 🔹 flex-basis

Sets initial size before growing/shrinking.

---

## 🔹 flex (shorthand)

```css
flex: 1;
```

Commonly used shortcut.

---

# 5️⃣ Why Flexbox is Powerful

✔ Easy horizontal alignment  
✔ Easy vertical centering  
✔ Flexible spacing  
✔ Responsive layouts  
✔ No float needed  

---

# 6️⃣ Most Common Pattern (Centering)

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

Perfectly centers content.

---

# Summary

- Flexbox = 1D layout system
- Works on main + cross axis
- Used for alignment & spacing
- Very powerful for UI layouts