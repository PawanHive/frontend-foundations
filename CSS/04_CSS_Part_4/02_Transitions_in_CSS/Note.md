# Transitions in CSS

## What is Transition?

A transition creates a **smooth animation effect**  
when a CSS property changes.

---

# 1️⃣ Basic Syntax

```css
transition: property duration timing-function delay;
```

Example:

```css
transition: all 0.3s ease;
```

---

# 2️⃣ Required Things

For transition to work:

- A property must change
- Usually triggered by `:hover`, `:focus`, or class change

Example:

```css
button {
  background: blue;
  transition: background 0.3s ease;
}

button:hover {
  background: red;
}
```

---

# 3️⃣ Transition Properties

## 🔹 transition-property

```css
transition-property: background;
```

Which property to animate.

---

## 🔹 transition-duration

```css
transition-duration: 0.5s;
```

How long animation runs.

---

## 🔹 transition-timing-function

Controls speed curve.

Common values:

- ease (default)
- linear
- ease-in
- ease-out
- ease-in-out

---

## 🔹 transition-delay

```css
transition-delay: 0.2s;
```

Wait before starting animation.

---

# 4️⃣ Multiple Properties

```css
transition: background 0.3s ease, transform 0.3s ease;
```

---

# 5️⃣ Common Animated Properties

✔ background-color  
✔ color  
✔ transform  
✔ opacity  
✔ box-shadow  

⚠ height and width can be animated but may cause layout issues.

---

# 6️⃣ Important Rules

- No change = no transition
- Works only between two states
- Must define transition on the initial state
- Use seconds (s) or milliseconds (ms)

---

# 7️⃣ Common Use Cases

- Button hover effects
- Smooth color change
- Card hover lift
- Fade in/out
- Menu animations

---

# Pro Developer Tip

Most common pattern:

```css
transition: all 0.3s ease;
```

But in real projects, prefer animating only needed properties.