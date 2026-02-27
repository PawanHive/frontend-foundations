# Alpha and Opacity in CSS

Both control transparency, but they work differently.

---

# 1️⃣ Opacity

```css
opacity: 0.5;
```

Range:
```
0 → fully transparent
1 → fully visible
```

## Important Rule

Opacity affects the **entire element**, including:

- Text
- Background
- Images
- Borders
- Children elements

If parent has:

```css
opacity: 0.5;
```

All children become transparent too.

---

# 2️⃣ Alpha (RGBA / HSLA)

Alpha controls transparency inside color values.

## Example (RGBA)

```css
background-color: rgba(255, 0, 0, 0.5);
```

Last value = alpha  
0 → transparent  
1 → solid  

## Example (HSLA)

```css
background-color: hsla(0, 100%, 50%, 0.5);
```

---

# Key Difference

| Property | Affects Whole Element? | Affects Only Color? |
|----------|------------------------|----------------------|
| opacity  | Yes                    | No                   |
| alpha    | No                     | Yes                  |

---

# When to Use Opacity

- Fade entire element
- Hover fade effects
- Animations

---

# When to Use Alpha

- Transparent background only
- Keep text fully visible
- Overlays

---

# Pro Tip

If you want:

Transparent background  
But solid text  

Use alpha (rgba/hsla), NOT opacity.