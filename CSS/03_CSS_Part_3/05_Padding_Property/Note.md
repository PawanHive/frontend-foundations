# Padding in CSS

## What is Padding?

Padding is the space **inside** an element, between the content and the border.

```
content → padding → border → margin
```

---

## 1️⃣ Basic Usage

```css
padding: 20px;
```

Adds 20px space on all 4 sides.

---

## 2️⃣ Four-Value Syntax

```css
padding: 10px 20px 30px 40px;
```

Order:

```
top → right → bottom → left
```

---

## 3️⃣ Two-Value Syntax

```css
padding: 10px 20px;
```

Means:

```
top & bottom = 10px
left & right = 20px
```

---

## 4️⃣ Three-Value Syntax

```css
padding: 10px 20px 30px;
```

Means:

```
top = 10px
left & right = 20px
bottom = 30px
```

---

## 5️⃣ Individual Sides

```css
padding-top: 10px;
padding-right: 20px;
padding-bottom: 30px;
padding-left: 40px;
```

---

## 6️⃣ Important Rules

- Padding increases total element size
- Background color extends into padding
- Padding cannot be negative
- Works on inline elements (but vertical padding may not push surrounding content properly)

---

## 7️⃣ Padding and Box Model

Default behavior:

```
total width = width + padding + border
total height = height + padding + border
```

Fix using:

```css
box-sizing: border-box;
```

---

## 8️⃣ Common Uses

- Space inside buttons
- Spacing inside cards
- Creating clickable area
- Making layouts breathable