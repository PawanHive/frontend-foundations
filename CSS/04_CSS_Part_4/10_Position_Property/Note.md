# CSS position

`position` controls how an element is placed in the document.

Values:

- static
- relative
- absolute
- fixed
- sticky

---

# 1️⃣ position: static (default)

```css
position: static;
```

- Default behavior
- Follows normal document flow
- top, left, right, bottom DO NOT work

---

# 2️⃣ position: relative

```css
position: relative;
top: 10px;
left: 20px;
```

- Stays in normal flow
- Can move using top, left, right, bottom
- Original space is still reserved

Used for:
- Small adjustments
- Parent for absolute elements

---

# 3️⃣ position: absolute

```css
position: absolute;
top: 0;
left: 0;
```

- Removed from normal flow
- No space reserved
- Positioned relative to nearest positioned ancestor
- If no positioned parent → relative to viewport

Important:
Parent must have:

```css
position: relative;
```

---

# 4️⃣ position: fixed

```css
position: fixed;
top: 0;
```

- Removed from normal flow
- Fixed relative to viewport
- Stays in same place while scrolling

Used for:
- Navbar
- Floating buttons

---

# 5️⃣ position: sticky

```css
position: sticky;
top: 0;
```

- Acts like relative at first
- Becomes fixed when scrolling reaches limit
- Needs top, left, right, or bottom value

Used for:
- Sticky headers
- Section titles

---

# Key Differences

| Value     | In Flow | Moves With Scroll | Needs Positioned Parent |
|-----------|---------|------------------|--------------------------|
| static    | Yes     | Yes              | No                       |
| relative  | Yes     | Yes              | No                       |
| absolute  | No      | Yes              | Yes                      |
| fixed     | No      | No               | No                       |
| sticky    | Yes     | Partially        | No                       |

---

# Important Rules

- top/left/right/bottom work only when position ≠ static
- absolute looks for nearest positioned ancestor
- fixed is always viewport-based
- sticky needs a scrollable container

---

# Pro Developer Tip

Most common pattern:

```css
.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 0;
  right: 0;
}
```

Very common in UI layouts.