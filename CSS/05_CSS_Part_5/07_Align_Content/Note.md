# align-content in Flexbox

## What is align-content?

`align-content` controls spacing between **multiple flex lines**  
along the **cross axis**.

⚠️ Important:  
It works **only when:**

- `flex-wrap: wrap;`
- There are multiple rows/columns
- There is extra space in the container

---

# 1️⃣ Important Difference

| Property | Works On |
|----------|----------|
| align-items | Individual items |
| align-content | Multiple lines (rows/columns) |

---

# 2️⃣ Default Value

```css
align-content: stretch;
```

Lines stretch to fill available space.

---

# 3️⃣ Common Values

## 🔹 stretch (default)

Lines stretch to fill cross axis.

---

## 🔹 flex-start

Lines packed at start of cross axis.

---

## 🔹 flex-end

Lines packed at end.

---

## 🔹 center

Lines centered in container.

---

## 🔹 space-between

Equal space between lines.

---

## 🔹 space-around

Equal space around lines.

---

## 🔹 space-evenly

Equal spacing everywhere.

---

# 4️⃣ Example

```css
.container {
  display: flex;
  flex-wrap: wrap;
  height: 300px;
  align-content: center;
}
```

All rows will be centered vertically  
(if direction is row).

---

# 5️⃣ When It Does NOT Work

❌ If there is only one line  
❌ If `flex-wrap: nowrap`  
❌ If there is no extra space  

---

# 6️⃣ Quick Visual Understanding

If:

```css
flex-direction: row;
```

Main axis = horizontal  
Cross axis = vertical  

So `align-content` controls vertical spacing between rows.

---

# Quick Summary

| Value          | Behavior |
|---------------|----------|
| stretch       | Fill container |
| flex-start    | Start |
| flex-end      | End |
| center        | Center |
| space-between | Equal space between lines |
| space-around  | Equal space around lines |
| space-evenly  | Equal space everywhere |