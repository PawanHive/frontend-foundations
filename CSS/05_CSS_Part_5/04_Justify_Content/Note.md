# justify-content in Flexbox

## What is justify-content?

`justify-content` controls alignment of flex items  
along the **main axis**.

It distributes extra space inside the flex container.

---

# 1️⃣ Important Rule

Main axis depends on `flex-direction`.

If:
```css
flex-direction: row;
```
Main axis = horizontal

If:
```css
flex-direction: column;
```
Main axis = vertical

---

# 2️⃣ Common Values

## 🔹 flex-start (default)

```css
justify-content: flex-start;
```

Items align at the start of main axis.

---

## 🔹 flex-end

```css
justify-content: flex-end;
```

Items align at the end.

---

## 🔹 center

```css
justify-content: center;
```

Items are centered.

---

## 🔹 space-between

```css
justify-content: space-between;
```

- First item at start  
- Last item at end  
- Equal space between items  

---

## 🔹 space-around

```css
justify-content: space-around;
```

Equal space around each item  
(edges get half space)

---

## 🔹 space-evenly

```css
justify-content: space-evenly;
```

Equal space everywhere (including edges).

---

# 3️⃣ Example

```css
.container {
  display: flex;
  justify-content: center;
}
```

Centers items along main axis.

---

# 4️⃣ Important Rules

- Works only on flex containers
- Controls main axis alignment
- Needs extra space to show effect
- Does not control cross axis

---

# Quick Summary

| Value          | Behavior |
|---------------|----------|
| flex-start    | Start |
| flex-end      | End |
| center        | Center |
| space-between | Equal space between |
| space-around  | Equal space around |
| space-evenly  | Equal space everywhere |