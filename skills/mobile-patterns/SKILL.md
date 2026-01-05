---
name: mobile-patterns
description: Cross-platform mobile development principles. State management, navigation, performance patterns.
---

# Mobile Patterns

> Core mobile development principles for React Native and Flutter.

---

## 1. State Management Selection

### By App Complexity

| Complexity | React Native | Flutter |
|------------|-------------|---------|
| Simple | Zustand | Provider |
| Medium | React Query + Zustand | Riverpod |
| Complex | Redux Toolkit | BLoC |

### Principles

- Server state ≠ UI state (separate them)
- Minimize global state
- Colocate state with components when possible
- Use reactivity, not manual updates

---

## 2. Navigation Principles

### Pattern Selection

| Need | Pattern |
|------|---------|
| Tab-based app | Tab navigator |
| Stack of screens | Stack navigator |
| Modal overlays | Modal presentation |
| Nested flows | Nested navigators |

### Best Practices

- Deep linking from day one
- Type-safe route params
- Handle back button (Android)
- Preserve state on tab switch

---

## 3. List Performance

### Optimization Principles

| Problem | Solution |
|---------|----------|
| Slow scrolling | Virtualized list |
| Re-renders | Memoize items |
| Jumpy scroll | Fixed item height |
| Memory | Remove off-screen items |

### Key Techniques

- Extract list items to separate components
- Use `memo` / `const` widgets
- Provide stable keys
- Avoid inline functions in render

---

## 4. API Integration

### Data Fetching Principles

| Pattern | Use When |
|---------|----------|
| **Query** | Read data |
| **Mutation** | Write data |
| **Subscription** | Real-time updates |

### Caching Strategy

- Cache server responses
- Invalidate on mutation
- Show stale while revalidating
- Handle offline gracefully

---

## 5. Storage Decision

| Data Type | Storage |
|-----------|---------|
| Tokens/secrets | Secure storage |
| User preferences | Async storage |
| Large/queryable | SQLite, Realm |
| Files | File system |

---

## 6. Platform Handling

### When to Diverge

| Aspect | Approach |
|--------|----------|
| Navigation gestures | Platform-default |
| Icons | Platform-specific |
| Date pickers | Platform-native |
| Core UI | Cross-platform |

### Principles

- iOS users expect iOS
- Android users expect Android
- Don't fight platform conventions

---

## 7. Anti-Patterns

| ❌ Don't | ✅ Do |
|----------|-------|
| One state for everything | Separate concerns |
| Re-render entire list | Memoize items |
| Sync calls in UI thread | Async operations |
| Ignore back button | Handle navigation |

---

> **Remember:** Mobile patterns exist because mobile is constrained. Respect the constraints.
