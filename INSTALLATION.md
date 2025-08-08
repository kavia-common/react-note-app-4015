# React Note App - Installation & Run Instructions

## Dependencies

The following core dependencies have been installed:
- `react`, `react-dom`: UI framework
- `react-router-dom`: Routing for protected/public routes
- `axios`: REST API integration
- `tailwindcss`, `postcss`, `autoprefixer`: CSS utility framework
- TypeScript & React types: Project is TypeScript-based
- Project supports React Context, hooks, and testing-library for testing

## Running the Application

### 1. Install (if you need to re-install)
```sh
yarn install
```

### 2. Running the Development Server

**Due to a known issue with Node.js v17+ and Webpack 4, you may see an error like:**
```
Error: error:0308010C:digital envelope routines::unsupported
```
**If this happens, run:**
```sh
export NODE_OPTIONS=--openssl-legacy-provider
yarn start
```
Or, prepend the variable inline:
```sh
NODE_OPTIONS=--openssl-legacy-provider yarn start
```

### 3. Build for Production
```sh
yarn build
```

---

## Notes

- All dependencies are already included in `package.json`.
- For REST API features, ensure your backend is running at `http://localhost:8080/api`.
- Tailwind CSS is integrated via scripts; see `package.json` for build details.

---
