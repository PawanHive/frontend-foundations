# border-radius in CSS

## What it does

Rounds the corners of an element.

---

## 1️⃣ Basic Usage

```css
border-radius: 10px;
```

Rounds all 4 corners equally.

---

## 2️⃣ Make a Circle

```css
border-radius: 50%;
```

⚠ Works only if:

- width = height  
- Element is square  

---

## 3️⃣ Different Values for Each Corner

```css
border-radius: 10px 20px 30px 40px;
```

Order:

```
top-left → top-right → bottom-right → bottom-left
```

---

## 4️⃣ Two-Value Shortcut

```css
border-radius: 10px 20px;
```

Means:

```
top-left & bottom-right = 10px
top-right & bottom-left = 20px
```

---

## 5️⃣ Individual Corners

```css
border-top-left-radius: 10px;
border-top-right-radius: 20px;
border-bottom-right-radius: 30px;
border-bottom-left-radius: 40px;
```

---

## 6️⃣ Elliptical Radius

```css
border-radius: 50px / 20px;
```

Creates oval corners.

Format:

```
horizontal-radius / vertical-radius
```

---

## 7️⃣ Important Rules

- Does NOT increase element size  
- Works with borders and background  
- Use overflow hidden for images inside rounded containers  

```css
overflow: hidden;
```

---

## 8️⃣ Common Uses

- Buttons  
- Cards  
- Avatars (circle images)  
- Modern UI components  