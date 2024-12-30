# React JS Performance Optimization Points

|   |   |
|---|---|
| **Lagezz** |   |

## Key Optimization Points

### 1. Code Splitting
Code splitting is a technique that involves dividing the JavaScript bundle into smaller chunks to load only the required code initially. This can be achieved using React's `React.lazy()` and `Suspense`.

### 2. Memoization
Memoization helps in optimizing React components by preventing unnecessary re-renders. Using hooks like `useMemo()` and `React.memo()` allows you to memoize values and components.

### 3. Avoid Inline Functions
Inline functions and objects are re-created with each render, which can cause unnecessary re-renders. It's recommended to move them outside of the render method or use hooks like `useCallback()`.

### 4. Lazy Loading of Images
Lazy loading of images means loading images only when they come into the viewport, thus reducing the initial load time of the page. You can use libraries like `react-lazyload` for this functionality.

### 5. Virtualization
For large lists or grids, virtualization renders only the visible items in the viewport, which improves performance. Libraries like `react-window` or `react-virtualized` are commonly used for this purpose.

### 6. Server-Side Rendering (SSR)
Server-side rendering (SSR) allows the server to render the React components and send the fully rendered page to the browser, improving the initial load time. Frameworks like `Next.js` support SSR out of the box.

### 7. Context API Optimization
Excessive use of the Context API can lead to unnecessary re-renders. It's better to optimize context usage or switch to state management libraries like `Redux` for complex applications.

### 8. Use of PureComponent
For class components, `PureComponent` can be used to prevent re-renders by performing shallow comparisons of props and state.

---

## Definitions for Key Topics

### Code Splitting
Code splitting is the practice of dividing a large JavaScript bundle into smaller chunks, which can be loaded dynamically as needed.

### Memoization
Memoization is an optimization technique where a function's results are cached, so the same calculations are not repeated.

### Virtualization
Virtualization refers to rendering only the visible content on the screen, such as a portion of a large list or grid, instead of rendering the entire content.

### Lazy Loading
Lazy loading is the technique of loading content (like images) only when it is needed or visible, instead of loading everything at once.
