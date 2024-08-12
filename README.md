Here’s a sample `README.md` file for your Vite project, detailing the setup and usage:

---

# Project

## Description

This is a Vite-based React project using TypeScript, Material-UI, and custom UI components. The project includes a basic setup with examples of text input, buttons, radio buttons, checkboxes, and dropdown lists.

## Features

- React with TypeScript
- Vite for fast development and build
- Material-UI for pre-built components
- Custom UI components (`ZText`, `ZButton`, `ZRadioGroup`, `ZCheckbox`, `ZSelect`)

## Setup

### Prerequisites

- Node.js (v14 or later)
- npm or Yarn

### Installation

1. **Clone the Repository**

   ```bash
   git clone <repository-url>
   cd vite-project
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

   or

   ```bash
   yarn install
   ```

3. **Run Development Server**

   ```bash
   npm run dev
   ```

   or

   ```bash
   yarn dev
   ```

   Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

### Project Structure

- `src/` - Contains the source code for the project.
  - `App.tsx` - Main application component.
  - `styles.css` - Global styles.
  - `ui-framework/` - Custom UI components and Material-UI integration.
    - `generic/` - Generic UI components like `Text`, `Checkbox`, etc.
    - `material-ui/` - Material-UI components like `Button`.

### Custom UI Components

#### `ZText`

A text input component with customizable properties.

**Usage:**

```tsx
import { ZText } from './ui-framework/generic/Text';

<ZText value={curName} onChange={(event) => setCurName(event.target.value)} />
```

#### `ZButton`

A button component with customizable properties.

**Usage:**

```tsx
import { ZButton } from './ui-framework/material-ui/Button';

<ZButton>Click Me</ZButton>
```

#### `ZRadioGroup`

A radio button group component.

**Usage:**

```tsx
import { ZRadioGroup } from './ui-framework/generic/RadioGroup';

<ZRadioGroup options={['Option 1', 'Option 2']} onChange={(event) => console.log(event.target.value)} />
```

#### `ZCheckbox`

A checkbox component.

**Usage:**

```tsx
import { ZCheckbox } from './ui-framework/generic/Checkbox';

<ZCheckbox checked={isChecked} onChange={(event) => setChecked(event.target.checked)} />
```

#### `ZSelect`

A dropdown select component.

**Usage:**

```tsx
import { ZSelect } from './ui-framework/generic/Select';

<ZSelect options={['Option 1', 'Option 2']} onChange={(event) => console.log(event.target.value)} />
```

## Configuration

- **Vite** - Configured for React and TypeScript. Check `vite.config.ts` for custom settings.
- **ESLint** - Configured for linting TypeScript and React code. Check `.eslintrc.json` for rule
