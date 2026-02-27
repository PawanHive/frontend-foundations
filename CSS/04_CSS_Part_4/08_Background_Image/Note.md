# CSS background-image

## What is background-image?

`background-image` sets an image as the background of an element.

---

# 1️⃣ Basic Syntax

```css
background-image: url("image.jpg");
```

---

# 2️⃣ Important Related Properties

## 🔹 background-size

```css
background-size: cover;
```

Common values:

- cover → fills element (may crop)
- contain → fits entire image (may leave space)
- 100% 100% → stretch

---

## 🔹 background-repeat

```css
background-repeat: no-repeat;
```

Values:

- repeat (default)
- no-repeat
- repeat-x
- repeat-y

---

## 🔹 background-position

```css
background-position: center;
```

Examples:

- center
- top
- bottom
- left
- right
- 50% 50%

---

## 🔹 background-attachment

```css
background-attachment: fixed;
```

Values:

- scroll (default)
- fixed (parallax effect)

---

# 3️⃣ Shorthand Property

```css
background: url("image.jpg") no-repeat center/cover;
```

Order (common pattern):

```
image → repeat → position/size
```

---

# 4️⃣ Multiple Background Images

```css
background-image: url("img1.png"), url("img2.png");
```

First image is on top.

---

# 5️⃣ Gradient as Background

```css
background: linear-gradient(to right, red, blue);
```

Gradients are also background images.

---

# Important Rules

- Background does NOT affect layout size
- By default, image repeats
- Use cover for hero sections
- Background stays inside padding area
- Works with border-radius

---

# Common Uses

- Hero sections
- Card backgrounds
- Overlay effects
- Pattern backgrounds
- Parallax sections