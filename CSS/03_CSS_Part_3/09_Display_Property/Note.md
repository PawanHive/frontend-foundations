# display Property in CSS

## What is display?

`display` controls **how an element behaves in layout**.

It decides:
- Block or inline behavior
- Whether it takes full width
- Whether width/height work
- How children are arranged

---

# 1️⃣ display: block

```css
display: block;
```

✔ Takes full width  
✔ Starts on new line  
✔ Width & height work  

Examples:
- div
- p
- h1–h6
- section

---

# 2️⃣ display: inline

```css
display: inline;
```

✔ Stays in same line  
❌ Width & height do NOT work  
❌ Top & bottom margin behave differently  

Examples:
- span
- a
- strong

---

# 3️⃣ display: inline-block

```css
display: inline-block;
```

✔ Stays inline  
✔ Width & height work  
✔ Margin & padding work properly  

Used for:
- Buttons
- Navbar items

---

# 4️⃣ display: none

```css
display: none;
```

✔ Removes element completely  
✔ Takes no space  
✔ Not visible  

---

# 5️⃣ display: flex

```css
display: flex;
```

✔ Creates flexible layout  
✔ Align children horizontally by default  
✔ Powerful alignment control  

Used for:
- Centering
- Navbars
- Layout sections

---

# 6️⃣ display: grid

```css
display: grid;
```

✔ 2D layout system  
✔ Rows + columns  
✔ Precise layout control  

Used for:
- Complex layouts
- Dashboards
- Galleries

---

# Important Rules

- Block = full width
- Inline = no width/height
- Inline-block = mix of both
- None = removed from layout
- Flex & Grid = layout systems

---

# Quick Comparison

| Type         | Full Width | Width/Height Work | New Line |
|-------------|------------|------------------|----------|
| block       | Yes        | Yes              | Yes      |
| inline      | No         | No               | No       |
| inline-block| No         | Yes              | No       |
| none        | No         | No               | No       |