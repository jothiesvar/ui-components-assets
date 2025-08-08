🎨 Free React Components Collection
A curated collection of modern, interactive React components built with TypeScript, Tailwind CSS, and shadcn/ui. All components are completely free to use in personal and commercial projects.

📋 Table of Contents
🚀 Quick Start
📦 Installation
🛠️ Implementation
📁 Components
⚙️ Requirements
🎯 Usage Examples
🤝 Contributing
📄 License
🚀 Quick Start
Get up and running in minutes! These components are designed to work seamlessly with modern React projects using shadcn/ui.

📦 Installation
Prerequisites
Make sure you have a React/Next.js project set up with:

✅ TypeScript
✅ Tailwind CSS
✅ shadcn/ui initialized
If you don't have these set up, follow the Project Setup section below.

Install Required Dependencies
bash
# Core dependencies for most components
npm install framer-motion @radix-ui/react-slot class-variance-authority

# Additional shadcn dependencies (if not already installed)
npm install lucide-react clsx tailwind-merge

# Component-specific dependencies (install as needed)
npm install @radix-ui/react-dialog @radix-ui/react-dropdown-menu
Project Setup
If you're starting from scratch:

bash
# Create new Next.js project
npx create-next-app@latest my-app --typescript --tailwind --eslint

# Navigate to your project
cd my-app

# Initialize shadcn/ui
npx shadcn@latest init
When prompted during shadcn init, use these recommended settings:

TypeScript: Yes
Tailwind CSS: Yes
src/ directory: Yes (recommended)
App Router: Yes
Import alias: @/*
🛠️ Implementation
Step 1: Create Required Files
Ensure you have the shadcn utility function:

lib/utils.ts

typescript
import { type ClassValue, clsx } from "clsx"
import { twMerge } from "tailwind-merge"

export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs))
}
Step 2: Copy Component Files
Copy the desired component from the /components folder
Place it in your components/ui/ directory
Install any component-specific dependencies listed in the component's README
Step 3: Import and Use
tsx
import { ComponentName } from "@/components/ui/component-name";

export default function Page() {
  return (
    <div>
      <ComponentName />
    </div>
  );
}
Step 4: Customize
Each component comes with customizable props and styling options. Check the individual component documentation for details.

📁 Components
Available Components
Component	Description	Dependencies	Demo
PhotoGallery	Interactive draggable image gallery with animations	framer-motion	View Demo
AnimatedButton	Smooth animated button with multiple variants	framer-motion	View Demo
LoadingSpinner	Beautiful loading animations	None	View Demo
ModalDialog	Accessible modal with backdrop	@radix-ui/react-dialog	View Demo
More components coming soon...

Component Features
🎯 Production Ready: Fully tested and optimized
📱 Responsive: Works perfectly on all device sizes
🌙 Dark Mode: Built-in dark/light theme support
♿ Accessible: WCAG compliant with proper ARIA attributes
🎨 Customizable: Easy to modify colors, sizes, and behavior
⚡ Performance: Optimized for speed and bundle size
⚙️ Requirements
System Requirements
Node.js: 16.8 or later
React: 18.0 or later
Next.js: 13.0 or later (recommended)
Required Dependencies
json
{
  "react": "^18.0.0",
  "react-dom": "^18.0.0",
  "typescript": "^5.0.0",
  "tailwindcss": "^3.3.0",
  "@types/react": "^18.0.0",
  "@types/react-dom": "^18.0.0"
}
🎯 Usage Examples
Basic Implementation
tsx
// app/page.tsx
import { PhotoGallery } from "@/components/ui/gallery";

export default function HomePage() {
  return (
    <main className="container mx-auto px-4">
      <h1 className="text-4xl font-bold text-center my-8">
        Welcome to My Portfolio
      </h1>
      <PhotoGallery animationDelay={0.3} />
    </main>
  );
}
With Custom Props
tsx
// components/custom-gallery.tsx
import { PhotoGallery } from "@/components/ui/gallery";

export function CustomGallery() {
  return (
    <div className="my-section">
      <PhotoGallery 
        animationDelay={0.5}
        // Add your custom props here
      />
    </div>
  );
}
Styling Customization
tsx
// You can customize components by:
// 1. Passing className props
// 2. Modifying the component's internal styles
// 3. Using CSS variables for theme colors

<PhotoGallery 
  className="my-custom-gallery" 
  animationDelay={0.2}
/>
🎨 Customization
Theming
All components support both light and dark themes out of the box. They automatically adapt to your shadcn/ui theme configuration.

Styling
Components use Tailwind CSS classes and can be easily customized by:

Modifying the component's CSS classes
Overriding styles with custom CSS
Using Tailwind's utility classes
Props
Each component accepts various props for customization. Check the component's TypeScript interface for all available options.

🤝 Contributing
We welcome contributions! Here's how you can help:

How to Contribute
Fork this repository
Clone your fork locally
Create a feature branch: git checkout -b feature/amazing-component
Commit your changes: git commit -m 'Add amazing component'
Push to the branch: git push origin feature/amazing-component
Open a Pull Request
Contribution Guidelines
✅ Follow TypeScript best practices
✅ Use Tailwind CSS for styling
✅ Include proper documentation
✅ Add component demos and examples
✅ Ensure accessibility compliance
✅ Test on different screen sizes
Component Requirements
When adding new components:

Must be built with TypeScript
Should support dark/light themes
Include proper prop interfaces
Add usage examples
Follow our naming conventions
📊 Stats
Show Image
Show Image
Show Image
Show Image

🆘 Support
Having issues? We're here to help!

📖 Check the documentation for detailed guides
🐛 Report bugs on GitHub
💬 Ask questions in Discussions
📧 Contact us at jothiesvar@gmail.com
📄 License
MIT License - You are free to use these components in personal and commercial projects.

MIT License

Copyright (c) 2024 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
⭐ Show Your Support
If you find these components helpful, please give this repository a star! ⭐

It helps others discover these free resources and motivates us to add more components.

<div align="center"> <strong>Built with ❤️ for the React community</strong><br> <sub>Happy coding! 🚀</sub> </div>
