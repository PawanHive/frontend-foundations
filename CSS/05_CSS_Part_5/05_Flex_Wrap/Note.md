# flex-wrap in Flexbox

## What is flex-wrap?

`flex-wrap` controls whether flex items:

- Stay in one single line  
OR  
- Move (wrap) to the next line when space is not enough  

---

# 1️⃣ Default Behavior

```css
flex-wrap: nowrap;
```

Items:

- Stay in one line
- Shrink to fit container
- Do NOT move to next line

---

# 2️⃣ flex-wrap Values

## 🔹 nowrap (default)

```css
flex-wrap: nowrap;
```

Everything stays in one row (or column).

---

## 🔹 wrap

```css
flex-wrap: wrap;
```

Items move to next line  
when there is no space.

Example (row direction):

```
Item1 Item2 Item3
Item4 Item5
```

---

## 🔹 wrap-reverse

```css
flex-wrap: wrap-reverse;
```

Items wrap in reverse direction.

New rows appear above (if row direction).

---

# 3️⃣ Important Rule

Wrap works based on main axis.

If:
```css
flex-direction: row;
```
→ wrapping happens to next row

If:
```css
flex-direction: column;
```
→ wrapping happens to next column

---

# 4️⃣ Common Usage

Usually used like this:

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

Very common for:
- Card layouts
- Image galleries
- Responsive designs

---

# 5️⃣ Shortcut Property

You can combine:

```css
flex-flow: row wrap;
```

`flex-flow = flex-direction + flex-wrap`

---

# Quick Summary

| Value        | Behavior |
|-------------|----------|
| nowrap      | Single line only |
| wrap        | Move to next line |
| wrap-reverse| Move in reverse direction |