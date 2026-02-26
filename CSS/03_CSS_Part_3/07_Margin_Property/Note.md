# Margin in CSS

## What is Margin?

Margin is the space **outside** an element, between the element and other elements.

```
content → padding → border → margin
```

---

## 1️⃣ Basic Usage

```css
margin: 20px;
```

Adds 20px space on all 4 sides.

---

## 2️⃣ Four-Value Syntax

```css
margin: 10px 20px 30px 40px;
```

Order:

```
top → right → bottom → left
```

---

## 3️⃣ Two-Value Syntax

```css
margin: 10px 20px;
```

Means:

```
top & bottom = 10px
left & right = 20px
```

---

## 4️⃣ Three-Value Syntax

```css
margin: 10px 20px 30px;
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
margin-top: 10px;
margin-right: 20px;
margin-bottom: 30px;
margin-left: 40px;
```

---

## 6️⃣ margin: auto (Centering Trick)

```css
margin: 0 auto;
```

✅ Centers block elements horizontally  
⚠ Requires:
- Fixed width
- display: block

---

## 7️⃣ Important Rules

- Margin can be negative
- Margin does NOT increase element size
- Background color does NOT extend into margin
- Vertical margins can collapse (between block elements)

---

## 8️⃣ Margin Collapsing

If two vertical margins touch:

```
margin-bottom: 20px;
margin-top: 30px;
```

Result = 30px (not 50px)

This happens only vertically.

---

## 9️⃣ Common Uses

- Spacing between sections
- Separating elements
- Centering layouts
- Creating layout gaps