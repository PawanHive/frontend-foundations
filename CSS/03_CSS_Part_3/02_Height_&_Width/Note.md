# Height in CSS – Important Rules

## 1️⃣ Default is `auto`

If you don’t set height, it grows based on content.

---

## 2️⃣ Percentage (%) Needs Parent Height

```css
.child {
  height: 100%;
}
```

✅ Works only if parent has a fixed/defined height.  
❌ If parent height is `auto`, this will not work.

---

## 3️⃣ Inline Elements Ignore Height

Inline elements like:

- span  
- a  
- strong  

do not respect `height`.

Fix:

```css
display: block;
```

or

```css
display: inline-block;
```

---

## 4️⃣ Content Can Overflow

If content is bigger than fixed height:

```css
height: 100px;
```

Content may overflow.

Control overflow using:

```css
overflow: hidden;
overflow: auto;
overflow: scroll;
```

---

## 5️⃣ Padding & Border Affect Total Height

Default behavior:

```
total height = height + padding + border
```

Fix using:

```css
box-sizing: border-box;
```

---

## 6️⃣ min-height Overrides height

```css
height: 100px;
min-height: 200px;
```

Final height = **200px**

---

## 7️⃣ max-height Limits Growth

```css
max-height: 300px;
```

Element will not exceed 300px even if content grows.

---

## 8️⃣ Flexbox Rule

If parent:

```css
display: flex;
```

Children stretch vertically by default because of:

```
align-items: stretch;
```

---

## 9️⃣ height: 100vh

- 100vh = 100% of viewport height
- Independent of parent
- Commonly used for full-screen sections

---

## 🔟 Avoid Fixed Height in Layouts

Instead prefer:

- padding
- min-height
- flexbox
- grid

Fixed height often breaks responsive design.