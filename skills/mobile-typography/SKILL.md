---
name: mobile-typography
description: Mobile typography principles. Type scale, readability, responsive text, dark mode.
---

# Mobile Typography

> Typography principles for mobile readability.

---

## 1. Mobile-Specific Considerations

| Factor | Impact |
|--------|--------|
| **Viewing distance** | Closer than desktop → larger base size |
| **Screen size** | Limited width → careful hierarchy |
| **Touch** | Labels need room |
| **Outdoor use** | Higher contrast needed |

---

## 2. Type Scale Principles

### Hierarchy

| Level | Use | Size Range |
|-------|-----|------------|
| Display | Hero, splash | 36-57px |
| Headline | Page titles | 24-32px |
| Title | Section, modal | 14-22px |
| Body | Content | 14-16px |
| Label | Buttons, tabs | 11-14px |
| Caption | Helper text | 11-12px |

### Scale Selection

- Use modular scale (1.25 for mobile)
- Limit to 5-7 sizes
- Be consistent across app

---

## 3. Minimum Sizes

| Purpose | Minimum |
|---------|---------|
| Body text | 14px |
| Captions | 11px |
| Nothing smaller | 11px |

### Why?

- Accessibility requirements
- Outdoor readability
- Aging user base

---

## 4. Line Height

| Text Type | Ratio |
|-----------|-------|
| Display | 1.1 |
| Headings | 1.25 |
| Body | 1.5 |
| Long-form | 1.75 |

---

## 5. Font Weight Usage

| Weight | Use |
|--------|-----|
| 400 (Regular) | Body, display |
| 500 (Medium) | Emphasis, buttons |
| 600 (Semibold) | Headings |
| 700 (Bold) | Rare, strong emphasis |

### Principle

- Avoid bold for body text
- Use weight for hierarchy, not decoration

---

## 6. System Fonts

### Platform Defaults

| Platform | Font |
|----------|------|
| iOS | San Francisco |
| Android | Roboto |

### When to Use System Fonts

- Faster load (no download)
- Platform consistency
- Accessibility features built-in

### When to Use Custom Fonts

- Strong brand identity
- Design requirement
- Consistent cross-platform look

---

## 7. Responsive Typography

### Principles

- Scale with screen width (within limits)
- Clamp between min and max
- Test on smallest and largest devices

### Breakpoint Approach

| Screen Width | Adjustment |
|--------------|------------|
| < 375px | Scale down 5-10% |
| 375-428px | Base size |
| > 428px | Scale up 5-10% |

---

## 8. Dark Mode Typography

### Color Adjustments

| Level | Light Mode | Dark Mode |
|-------|------------|-----------|
| Primary | #000000 | #FFFFFF |
| Secondary | #666666 | #E3E3E3 |
| Tertiary | #999999 | #A0A0A0 |

### Principles

- Reduce pure white (#FFF → #E3E3E3)
- Increase contrast for readability
- Test both modes

---

## 9. Anti-Patterns

| ❌ Don't | ✅ Do |
|----------|-------|
| Font size < 11px | Min 11px |
| Bold body text | Regular or medium |
| Too many sizes | 5-7 sizes max |
| Line height 1.0 | Min 1.25 for body |
| Ignore dark mode | Design for both |

---

## 10. Quick Reference

| Style | Size | Weight | Line Height |
|-------|------|--------|-------------|
| Display | 45-57 | 400 | 1.1 |
| Headline | 24-32 | 400-600 | 1.25 |
| Title | 16-22 | 500 | 1.25 |
| Body | 14-16 | 400 | 1.5 |
| Label | 12-14 | 500 | 1.25 |
| Caption | 11-12 | 400 | 1.33 |

---

> **Remember:** Mobile reading is harder. Bigger text, more contrast, more space.
