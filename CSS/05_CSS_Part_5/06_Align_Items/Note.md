# align-items in Flexbox

## What is align-items?

`align-items` controls alignment of flex items  
along the **cross axis**.

It aligns items inside the flex container.

---

# 1️⃣ Important Rule

Cross axis depends on `flex-direction`.

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

---

# 2️⃣ Default Value

```css
align-items: stretch;
```

Items stretch to fill the container  
(if no height/width is fixed).

---

# 3️⃣ Common Values

## 🔹 stretch (default)

```css
align-items: stretch;
```

Items expand to fill cross axis.

---

## 🔹 flex-start

```css
align-items: flex-start;
```

Items align at start of cross axis.

---

## 🔹 flex-end

```css
align-items: flex-end;
```

Items align at end of cross axis.

---

## 🔹 center

```css
align-items: center;
```

Items align at center of cross axis.

---

## 🔹 baseline

```css
align-items: baseline;
```

Items align according to text baseline.

Useful when items have different font sizes.

---

# 4️⃣ Example

```css
.container {
  display: flex;
  height: 200px;
  align-items: center;
}
```

Items will be vertically centered  
(if direction is row).

---

# 5️⃣ Difference From justify-content

| Property | Controls |
|----------|----------|
| justify-content | Main axis |
| align-items | Cross axis |

---

# Quick Summary

| Value      | Behavior |
|-----------|----------|
| stretch   | Fill container |
| flex-start| Start |
| flex-end  | End |
| center    | Center |
| baseline  | Text baseline |