---
name: mobile-ux-patterns
description: Mobile UX principles. Touch gestures, haptic feedback, accessibility, touch targets.
---

# Mobile UX Patterns

> Touch-first UX principles for mobile apps.

---

## 1. Touch Target Principles

### Minimum Sizes

| Element | Minimum | Recommended |
|---------|---------|-------------|
| Buttons | 44pt | 48pt |
| Icons | 24pt | 32pt |
| List items | 44pt height | 48-56pt |
| Spacing | 8pt | 12pt |

### Why It Matters

- Thumbs are imprecise
- Touch occludes the target
- Error taps frustrate users

---

## 2. Gesture Selection

### Common Gestures

| Gesture | Use For |
|---------|---------|
| **Tap** | Primary action |
| **Long press** | Context menu, selection |
| **Swipe** | Delete, actions, navigation |
| **Pinch** | Zoom |
| **Double tap** | Quick action (like) |
| **Pull down** | Refresh |

### Gesture Principles

- Gestures need discoverability
- Always provide alternative actions
- Provide feedback during gesture
- Respect platform conventions

---

## 3. Haptic Feedback

### When to Use

| Intensity | Use Case |
|-----------|----------|
| Light | Selection, toggle |
| Medium | Action confirmed |
| Heavy | Important action |
| Success | Completion |
| Warning | Error, attention |

### Principles

- Less is more
- Match intensity to action importance
- Don't use for every tap
- Respect user settings

---

## 4. Pull to Refresh

### Best Practices

- Clear visual indicator
- Don't block content during refresh
- Show timestamp of last refresh
- Handle errors gracefully

---

## 5. Swipe Actions

### Design Principles

| Aspect | Guideline |
|--------|-----------|
| Direction | Left = destructive, Right = constructive |
| Reveal | Show action icons behind content |
| Threshold | 30-40% of width to trigger |
| Confirmation | Destructive actions need confirmation |

---

## 6. Accessibility

### Required Elements

| Element | Requirement |
|---------|------------|
| Labels | Every interactive element |
| Roles | Button, link, heading, etc. |
| Hints | How to use if not obvious |
| Actions | Alternative to gestures |

### Testing

- Enable VoiceOver/TalkBack
- Navigate without seeing screen
- Test with larger text
- Check color contrast

---

## 7. Loading States

### Types

| State | Pattern |
|-------|---------|
| Initial load | Skeleton |
| Refresh | Pull indicator |
| Submit | Button loading |
| Navigation | Progress bar |

### Principles

- Never leave user wondering
- Show progress when possible
- Allow cancellation for long operations

---

## 8. Anti-Patterns

| ❌ Don't | ✅ Do |
|----------|-------|
| Small touch targets | Min 44pt |
| Gestures without alternative | Provide buttons |
| Haptics on every tap | Strategic haptics |
| No loading states | Always show progress |
| Skip accessibility | Full a11y support |

---

> **Remember:** Touch is imprecise. Design for thumbs, not cursors.
