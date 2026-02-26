# Border in CSS

## What is Border?

Border draws a line around an element.

---

## 1️⃣ Basic Syntax

```css
border: 2px solid black;
```

Shorthand for:

```css
border-width: 2px;
border-style: solid;
border-color: black;
```

---

## 2️⃣ Border Properties

### 🔹 border-width

```css
border-width: 4px;
```

Defines thickness of the border.

---

### 🔹 border-style (Required)

```css
border-style: solid;
```

Common values:

- solid
- dashed
- dotted
- double
- none

⚠ Without `border-style`, border will not appear.

---

### 🔹 border-color

```css
border-color: red;
```

Defines border color.

---

## 3️⃣ Side-Specific Borders

```css
border-top: 2px solid red;
border-right: 2px solid blue;
border-bottom: 2px solid green;
border-left: 2px solid black;
```

Or individual properties:

```css
border-top-width: 5px;
```

---

## 4️⃣ Border Radius (Rounded Corners)

```css
border-radius: 10px;
```

Circle:

```css
border-radius: 50%;
```

---

## 5️⃣ Border and Box Model

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

## 6️⃣ Transparent Border Trick

```css
border: 2px solid transparent;
```

Used for hover effects to prevent layout shift.

---

## 7️⃣ Outline vs Border

```css
outline: 2px solid red;
```

Difference:

- Border takes space
- Outline does NOT take space
- Outline is commonly used for focus states

---

## 8️⃣ Important Rules

- Border increases element size (unless using border-box)
- border-style is mandatory
- You can use shorthand or individual properties
- Each side can be styled differently