# React Hamster Loading

A cute animated hamster running in a wheel loading spinner component for React applications.

![Hamster Loading Animation](https://img.shields.io/badge/React-Component-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-Ready-green)
![Styled Components](https://img.shields.io/badge/Styled--Components-Powered-purple)

## Installation

```bash
npm install @lcaohoanq/react-hamster-loading
```

or

```bash
yarn add @lcaohoanq/react-hamster-loading
```

## Usage

### Basic Usage

```tsx
import React from "react";
import { LoadingHamster } from "@lcaohoanq/react-hamster-loading";

function App() {
  return (
    <div>
      <h1>Loading...</h1>
      <LoadingHamster />
    </div>
  );
}

export default App;
```

### As Default Import

```tsx
import React from "react";
import LoadingHamster from "@lcaohoanq/react-hamster-loading";

function MyComponent() {
  const [loading, setLoading] = React.useState(true);

  if (loading) {
    return <LoadingHamster />;
  }

  return <div>Content loaded!</div>;
}
```

## Features

- 🐹 Cute animated hamster running in a wheel
- ⚡ Lightweight and performant
- 🎨 Styled with styled-components
- 📱 Responsive design
- 🔧 TypeScript support
- 🎯 Zero dependencies (except peer dependencies)
- ♿ Accessible with proper ARIA labels

## Peer Dependencies

This package requires the following peer dependencies:

- `react` >= 16.8.0
- `react-dom` >= 16.8.0
- `styled-components` >= 5.0.0

## Component Props

The `LoadingHamster` component currently doesn't accept any props and displays with default styling. Future versions may include customization options.

## Customization

The component uses CSS custom properties internally. You can override the animation duration by wrapping it in a styled component:

```tsx
import styled from "styled-components";
import { LoadingHamster } from "@lcaohoanq/react-hamster-loading";

const CustomHamster = styled(LoadingHamster)`
  .wheel-and-hamster {
    --dur: 2s; /* Slower animation */
  }
`;
```

## Browser Support

This component works in all modern browsers that support:

- CSS animations
- CSS custom properties (variables)
- ES6+ features

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Created by [lcaohoanq](https://github.com/lcaohoanq)

## Changelog

### 1.0.0

- Initial release
- Basic hamster loading animation
- TypeScript support
- Styled-components integration
  })

````

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
````
