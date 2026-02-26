# Percentage (%) Unit in CSS

## What is % ?

`%` is a relative unit.

It is calculated based on the size of the **parent element**.

---

# 1️⃣ Width with %

```css
width: 50%;
```

Element takes 50% of the parent’s width.

✅ Very common  
✅ Good for responsive layouts  

---

# 2️⃣ Height with %

```css
height: 50%;
```

⚠ Works ONLY if parent has a defined height.

If parent height is `auto`, this will not work properly.

---

# 3️⃣ Padding with %

```css
padding: 10%;
```

Important rule:

👉 Percentage padding is based on **parent's width**,  
NOT height.

Even `padding-top` and `padding-bottom` use width.

---

# 4️⃣ Margin with %

```css
margin: 5%;
```

Also based on **parent's width**.

---

# 5️⃣ Font Size with %

```css
font-size: 120%;
```

Based on parent’s font size.

Example:
- Parent = 16px  
- 120% = 19.2px  

---

# 6️⃣ Positioning with %

```css
left: 50%;
top: 50%;
```

Calculated relative to the positioned parent.

---

# Important Rules

- % is always relative to something
- Usually relative to parent
- Height % needs parent height
- Padding % is based on width
- Makes layouts responsive

---

# When to Use %

- Responsive widths
- Flexible layouts
- Fluid containers
- Scalable typography