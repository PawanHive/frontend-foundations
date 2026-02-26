# em and rem Units in CSS

Both `em` and `rem` are relative units used mainly for:

- font-size
- spacing
- layout scaling

---

# 1️⃣ em Unit

`em` is relative to the **font-size of the parent element**.

## Example

```css
.parent {
  font-size: 20px;
}

.child {
  font-size: 2em;   /* 40px */
}
```

2em = 2 × parent font-size

---

## Important Rule of em

⚠ em can compound (multiply).

If:

```css
.parent {
  font-size: 20px;
}

.child {
  font-size: 2em;   /* 40px */
}

.grandchild {
  font-size: 2em;   /* 80px */
}
```

It keeps multiplying.

This can cause unexpected scaling.

---

# 2️⃣ rem Unit

`rem` = **root em**

It is always relative to the `<html>` font-size.

Default browser root font-size = 16px

## Example

```css
html {
  font-size: 16px;
}

p {
  font-size: 2rem;   /* 32px */
}
```

2rem = 2 × root font-size

---

# Key Difference

| Unit | Based On | Compounds? |
|------|----------|------------|
| em   | Parent   | Yes        |
| rem  | Root     | No         |

---

# When to Use em

- Button padding relative to its text
- Components that scale internally

---

# When to Use rem

- Global font sizing
- Layout spacing
- Consistent scaling across project

---

# Pro Developer Rule

Use:
- rem → for most font sizes and spacing
- em → inside components

Avoid deep nesting with em.