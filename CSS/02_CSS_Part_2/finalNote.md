# #1: Pseudo-Class in CSS

## MDN Link: [Pseudo-Class](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Selectors/Pseudo-classes)

A **pseudo-class** is used to define the **special state** of an element.

It starts with a **colon (`:`)**.

---

## 🔹 Basic Syntax

```css
selector:pseudo-class {
  property: value;
}
```

---

## 🎯 What Is a "State"?

A state means:

- When a user hovers over an element
- When an input is focused
- When a link is visited
- When an element is the first child
- When a button is being clicked

---

## 🔥 Common Pseudo-Classes (Very Important)

### 1️⃣ `:hover`

Applies style when the mouse is over an element.

```css
button:hover {
  background-color: red;
}
```

---

### 2️⃣ `:active`

Applies style when the element is being clicked.

```css
button:active {
  background-color: green;
}
```

---

### 3️⃣ `:focus`

Applies style when an input field is selected.

```css
input:focus {
  border: 2px solid blue;
}
```

---

### 4️⃣ `:visited`

Applies style to visited links.

```css
a:visited {
  color: purple;
}
```

---

### 5️⃣ `:first-child`

Selects the first child element.

```css
li:first-child {
  color: red;
}
```

---

### 6️⃣ `:last-child`

Selects the last child element.

```css
li:last-child {
  color: blue;
}
```

---

### 7️⃣ `:nth-child()`

Selects an element based on its position.

```css
li:nth-child(2) {
  color: green;
}
```

Even elements:

```css
li:nth-child(even)
```

Odd elements:

```css
li:nth-child(odd)
```

---

## 🧠 Important Difference

### Pseudo-class
Uses a single colon:

```
:
```

Example:

```css
button:hover
```

---

### Pseudo-element
Uses double colon:

```
::
```

Examples:

```css
p::first-letter
```
```css
p::first-line
```
```css
p::selection
```

---

## 📌 Simple Definition (Exam Friendly)

> A pseudo-class is used to define a special state of an HTML element.

---

## 🚀 Real Example

### HTML

```html
<button>Click Me</button>
```

### CSS

```css
button:hover {
  background-color: black;
  color: white;
}
```

When you move the mouse over the button, the style changes.

---

# #2: Specificity Calculation Trick

CSS calculates specificity like this:

```
(ID, Class, Element)
```
means: **Id** > **class, pseudo-class** > **element, pseudo-element**
- `id` has highest specificiy and `element` has lowest specificity
---

### Example

```css
#main .box p
```

### Specificity Calculation

```
(1, 1, 1)
```

- 1 ID  
- 1 Class  
- 1 Element  

---


## 🚀 Real-Life Understanding

Think of specificity like a priority system:

- **ID** = VIP  
- **Class** = Important person  
- **Element** = Normal person  
- **`!important`** = Emergency override  

VIP always wins.
