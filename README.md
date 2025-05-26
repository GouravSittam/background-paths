# Background Paths

A beautiful and interactive React component library to render animated background lines and gradient text for modern web applications.

![Preview](https://github.com/GouravSittam/background-paths/raw/main/preview.png)

## ✨ Features

- **Animated SVG Paths:** Generates 36 random animated SVG lines as a stylish background.
- **Gradient Text Animation:** Each letter in the title animates in with a spring effect and a smooth gradient.
- **Dark Mode Support:** Automatically adapts to dark and light themes using Tailwind CSS and custom CSS variables.
- **Customizable:** Easily change background and foreground colors, gradients, and path effects.
- **Built with React & Framer Motion:** Smooth, performant animations for interactive UIs.

## 🚀 Demo

```tsx
import BackgroundPaths from "./components/kokonutui/background-paths";

export default function App() {
  return <BackgroundPaths title="Your Awesome Title" />;
}
```

## 🛠️ How it Works

- **`BackgroundPaths` Component:** Renders a full-screen flex container with animated floating SVG paths in the background and a centered animated gradient title.
- **`FloatingPaths` Subcomponent:** Randomly generates and animates SVG lines for a dynamic, ever-changing background.
- **Button:** Includes a call-to-action button with hover effects.
- **Styling:** Uses Tailwind CSS and custom variables for easy theming.

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/GouravSittam/background-paths.git
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Run the app:**
   ```bash
   npm run dev
   ```

## 🎨 Customization

- **Change title text:** Pass a custom `title` prop to `<BackgroundPaths />`.
- **Adjust theme:** Edit `app/globals.css` or `tailwind.config.ts` for custom colors and gradients.
- **Modify line count/effects:** Tweak the `FloatingPaths` function in `components/kokonutui/background-paths.tsx`.

## 🏗️ Architecture

The **Background Paths** project is designed as a modular React component library with a clear separation of concerns for maximum reusability and theming flexibility. Here’s an overview of its architecture:

### Core Components

- **`BackgroundPaths`**  
  The main entry component that renders the animated background and gradient title.  
  - Uses `FloatingPaths` internally for SVG background lines.
  - Handles layout, theming (light/dark), and the main call-to-action button.

- **`FloatingPaths`**  
  A utility subcomponent inside `BackgroundPaths` responsible for generating and animating multiple SVG line elements.  
  - Randomly generates coordinates and styles for each animated path.
  - Uses Framer Motion for smooth, infinite SVG animations.

- **`Button`**  
  A styled button used for the call-to-action, themed with Tailwind CSS and custom classes.

### Styling & Theming

- **Tailwind CSS**:  
  All components use Tailwind CSS utility classes for rapid styling and easy theme switching.
- **Custom CSS Variables**:  
  The project leverages CSS variables in `globals.css` for consistent color themes and gradients, including dark mode support.

### File Structure

```
/app
  └── page.tsx                # Demo/entry page
/components
  └── kokonutui/
      └── background-paths.tsx  # Main animated component
/app/globals.css              # Global styles and theming
/tailwind.config.ts           # Tailwind configuration and theme extension
```

### Animation

- **Framer Motion**:  
  Provides advanced animation capabilities for SVG paths and text elements, ensuring performant and visually appealing transitions.

---

This architecture ensures the library is easy to extend, theme, and integrate into any modern React application.


## 📄 License

This project is open-source. See [LICENSE](LICENSE) for details.

---

Crafted with ❤️ by [Gourav Sittam](https://github.com/GouravSittam)
