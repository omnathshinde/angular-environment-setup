# 🚀 Angular Project

This is a modular Angular application following best practices with environment-based configurations, Prettier formatting, and ready-to-use commands for development, staging, and production.

---

## 📁 Project Setup

1. **Install dependencies**

    ```bash
    npm install
    ```

2. **Code Formatting**

    Format your code using Prettier before committing:

    ```bash
    npm run format
    ```

---

## 🌐 Serve the Application

### Development

```bash
ng serve --open
```

```bash
ng serve --configuration=development
```

### Staging

```bash
ng serve --configuration=staging
```

### Production

```bash
ng serve --configuration=production
```

---

## 🏗️ Build the Application

### Development Build

```bash
ng build --configuration=development
```

### Staging Build

```bash
ng build --configuration=staging
```

### Production Build

```bash
ng build --configuration=production
```

---

## 🌎 Environment Files

Environment-specific configuration files are located in:

```
src/environments/
├── environment.ts              # Default (development)
├── environment.stag.ts         # Staging
└── environment.prod.ts         # Production
```

To add custom variables, update these files and reference via `environment.<key>` after importing:

```ts
import { environment } from "src/environments/environment";

console.log(environment.apiUrl);
```

---

## ✅ Pre-push Checklist

Before pushing your code to the repository:

- [ ] ✅ Format your code: `npm run format`
- [ ] ✅ Test locally with `ng serve --configuration=<env>`
- [ ] ✅ Ensure environment variables are correctly configured
- [ ] ✅ Verify there are no build errors

---

## 📦 Scripts Overview

| Script           | Description                    |
| ---------------- | ------------------------------ |
| `npm run format` | Format all code using Prettier |
| `ng serve`       | Run local dev server           |
| `ng build`       | Build the app for deployment   |

---

Feel free to update this README as your project evolves. Happy coding! 💻✨
