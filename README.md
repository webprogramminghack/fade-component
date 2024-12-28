# FadeWrapper Component

The `FadeWrapper` component is a reusable React component that provides a dynamic fade effect for its children. It supports both horizontal and vertical fades, with fully customizable colors and widths.

## Features

- **Horizontal and Vertical Fades**: Supports fades on the `start`, `end`, or both directions for horizontal and vertical layouts.
- **Customizable Fade Color**: Dynamically set the gradient color using the `fadeColor` prop.
- **Adjustable Fade Width**: Control the width or height of the fade using the `fadeWidth` prop.
- **Smooth Transitions**: Leverages `framer-motion` for smooth animations on visibility changes.

## Watch This Video

[https://youtu.be/XT_z85D8eNU](https://youtu.be/XT_z85D8eNU)

## Installation

To use the `FadeWrapper` component, ensure you have the following dependencies installed:

```bash
npm install framer-motion clsx
```

## Usage Example

```javascript
import React from 'react';
import { FadeWrapper } from './FadeWrapper';

const App = () => {
  return (
    <FadeWrapper
      type='both' // Fade direction: 'start', 'end', 'both', or 'none'
      direction='horizontal' // Orientation: 'horizontal' or 'vertical'
      fadeWidth={128} // Width or height of the fade (in pixels)
      fadeColor='#ff0000' // Custom fade color
    >
      <p>This content fades with a red gradient!</p>
    </FadeWrapper>
  );
};

export default App;
```
