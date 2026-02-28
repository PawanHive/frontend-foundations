# display: flex

## What does display: flex do?

```css
display: flex;
```

It turns an element into a **flex container**.

All its direct children become **flex items**.

---

# 1️⃣ Default Behavior

When you apply:

```css
.container {
  display: flex;
}
```

By default:

- Items align in a row (left → right)
- Items stay in one line
- Items stretch vertically
- Space is distributed automatically

Default values:

```
flex-direction: row;
justify-content: flex-start;
align-items: stretch;
flex-wrap: nowrap;
```

---

# 2️⃣ Main Axis & Cross Axis

Flexbox works on two axes:

- Main Axis → controlled by flex-direction
- Cross Axis → perpendicular to main axis

If direction is row:
- Main = horizontal
- Cross = vertical

If direction is column:
- Main = vertical
- Cross = horizontal

---

# 3️⃣ What Happens to Children?

Flex items:

✔ Sit in one line (by default)  
✔ Can shrink to fit container  
✔ Can grow if allowed  
✔ Ignore vertical margin collapse  

---

# 4️⃣ Most Used Properties After display: flex

## 🔹 justify-content
Controls alignment on main axis.

## 🔹 align-items
Controls alignment on cross axis.

## 🔹 flex-wrap
Allows items to move to next line.

## 🔹 gap
Adds spacing between items.

---

# 5️⃣ Common Example

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

This perfectly centers content.

---

# 6️⃣ Important Rules

- Only direct children become flex items
- Flexbox is 1-dimensional
- Great for horizontal layouts
- Removes need for float

---

# When to Use display: flex

- Navbar
- Button groups
- Card layouts
- Centering elements
- Layout alignment