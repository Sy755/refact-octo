# Naming Conventions Guide

This document provides guidelines for choosing descriptive variable and function names in your code.

## Variable Naming

### Use Descriptive Names
- **Avoid**: `x`, `n`, `temp`, `data`
- **Prefer**: `userAge`, `itemCount`, `temporaryBuffer`, `userData`

### Be Specific About Content
- **Avoid**: `list`, `arr`, `obj`
- **Prefer**: `userList`, `productPrices`, `userProfile`

### Use Consistent Casing
- **camelCase** for variables: `userName`, `isActive`, `totalPrice`
- **UPPER_SNAKE_CASE** for constants: `MAX_RETRY_COUNT`, `API_BASE_URL`

### Include Units When Relevant
- **Avoid**: `timeout`, `distance`, `size`
- **Prefer**: `timeoutMs`, `distanceKm`, `fileSizeBytes`

## Function Naming

### Use Verb-Based Names
Functions perform actions, so start with a verb:
- **Avoid**: `password()`, `user()`
- **Prefer**: `validatePassword()`, `fetchUser()`

### Common Verb Prefixes
| Prefix | Usage | Example |
|--------|-------|---------|
| `get` | Retrieve a value | `getUserName()` |
| `set` | Assign a value | `setUserName()` |
| `is` / `has` | Boolean check | `isActive()`, `hasPermission()` |
| `validate` | Check validity | `validateEmail()` |
| `create` | Instantiate new | `createUser()` |
| `update` | Modify existing | `updateProfile()` |
| `delete` | Remove | `deleteAccount()` |
| `fetch` | Retrieve from external source | `fetchUserData()` |
| `calculate` | Compute a value | `calculateTotal()` |
| `format` | Transform display | `formatDate()` |

### Be Specific About What the Function Does
- **Avoid**: `process()`, `handle()`, `do()`
- **Prefer**: `processPayment()`, `handleFormSubmission()`, `executeQuery()`

## Boolean Variables

Use prefixes that indicate a yes/no question:
- `is`: `isVisible`, `isEnabled`, `isLoggedIn`
- `has`: `hasChildren`, `hasErrors`, `hasPermission`
- `can`: `canEdit`, `canDelete`, `canSubmit`
- `should`: `shouldUpdate`, `shouldNotify`

## Examples

### Before (Poor Naming)
```javascript
function calc(a, b) {
  const x = a * b;
  return x;
}

let d = getData();
let flag = true;
```

### After (Descriptive Naming)
```javascript
function calculateRectangleArea(width, height) {
  const area = width * height;
  return area;
}

let userData = fetchUserProfile();
let isFormValid = true;
```

## Summary

Good variable and function names should:
1. Clearly describe their purpose
2. Be readable without additional context
3. Follow consistent conventions
4. Avoid abbreviations unless widely understood
