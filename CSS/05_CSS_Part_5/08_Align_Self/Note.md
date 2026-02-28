# align-self in Flexbox

## What is align-self?

`align-self` controls alignment of a **single flex item**  
along the **cross axis**.

It overrides `align-items` for one item.

---

# 1️⃣ Important Rule

`align-self` works on:

✔ Individual flex items  
❌ Not on the flex container  

---

# 2️⃣ Cross Axis Reminder

If:
```css
flex-direction: row;
```
Main axis = horizontal  
Cross axis = vertical  

If:
```css
flex-direction: column;
```
Main axis = vertical  
Cross axis = horizontal  

`align-self` works on the cross axis.

---

# 3️⃣ Default Value

```css
align-self: auto;
```

It follows the container's `align-items` value.

---

# 4️⃣ Common Values

## 🔹 auto (default)

Follows `align-items`.

---

## 🔹 flex-start

Item moves to start of cross axis.

---

## 🔹 flex-end

Item moves to end of cross axis.

---

## 🔹 center

Item moves to center.

---

## 🔹 stretch

Item stretches to fill cross axis.

---

## 🔹 baseline

Aligns based on text baseline.

---

# 5️⃣ Example

```css
.container {
  display: flex;
  align-items: center;
}

.item2 {
  align-self: flex-end;
}
```

All items → center  
Only `.item2` → moves to end  

---

# 6️⃣ When To Use It

Use `align-self` when:

- You want one item different
- You don’t want to change all items

---

# Quick Difference

| Property      | Works On |
|--------------|----------|
| align-items  | All items |
| align-self   | One item only |