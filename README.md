# Reuse - Sustainable Marketplace

![Reuse Platform Screenshot](./assets/images/screenshot.png)

## Description

Reuse is a modern e-commerce marketplace designed to promote sustainability by facilitating the buying, selling, and trading of pre-owned items. The platform aims to revolutionize how people think about waste and sustainability by connecting individuals and businesses, encouraging reuse to reduce waste and promote a circular economy.

## Mission & Vision

Our mission is to create a world where sustainability is the norm, not the exception, by making reuse easy, accessible, and impactful for both individuals and businesses. We envision a future where waste is a thing of the past, and every resource is valued and utilized to its fullest potential.

## Features

- **User Authentication**: Secure sign-up and login functionality
- **Multi-language Support**: Interface available in English, German, and French
- **Product Categories**: Browse items by multiple categories (Electronics, Fashion, Home & Garden, Motors, etc.)
- **Advanced Search**: Filter products by category, location, and keywords
- **Shopping Cart**: Add, view, and checkout items
- **Seller Dashboard**: List and manage items for sale
- **Interactive Chat Bot**: Get assistance and support via the Reuse chat bot
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Rating System**: View product ratings and reviews
- **Location-based Filtering**: Search by city and zip code
- **Educational Content**: Learn about sustainability and the circular economy

## Technologies Used

### Frontend
- **React** - Component-based UI development
- **Vite** - Next-generation frontend tooling
- **React Router** - Navigation and routing
- **Framer Motion** - Animations and transitions
- **Tailwind CSS** - Utility-first CSS framework
- **DaisyUI** - Tailwind CSS component library
- **Axios** - Promise-based HTTP client
- **Cloudinary Video Player** - For media content delivery

### Backend
- Node.js (Express)
- MongoDB
- JWT Authentication
- RESTful API Architecture

## Installation

Follow these steps to set up the client-side application locally:

```bash
# Clone the repository
git clone <your-repo-url>

# Navigate to the project directory
cd Reuse/Client

# Install dependencies
npm install

# If you encounter issues with framer-motion, use this specific version
npm uninstall framer-motion
npm install framer-motion@10.16.4
```

## Configuration

If you encounter module resolution errors with framer-motion, update your `vite.config.js` file:

```javascript
import { defineConfig } from "vite";
import react from "@vitejs/plugin-react";

export default defineConfig({
  plugins: [react()],
  optimizeDeps: {
    include: ['framer-motion']
  },
  build: {
    commonjsOptions: {
      transformMixedEsModules: true
    }
  }
});
```

## Usage

To start the development server:

```bash
npm run dev
```

To build for production:

```bash
npm run build
```

To preview the production build:

```bash
npm run preview
```

## How Reuse Works

At Reuse, we aim to revolutionize the way people think about waste and sustainability. Our platform connects individuals and businesses to facilitate the buying, selling, and trading of reusable items. By encouraging reuse, we reduce waste and promote a circular economy where resources are maximized and waste is minimized.

Our philosophy centers around sustainability, community, and innovation. We believe in giving a second life to products that would otherwise be discarded. Through our platform, we empower individuals to make environmentally conscious decisions and inspire a culture of reuse that benefits everyone.

## Troubleshooting

If you encounter dependency issues:

1. Try removing the `motion` package if it's installed alongside `framer-motion`
2. Use a stable version of framer-motion (10.16.4 recommended)
3. Clear node_modules and reinstall dependencies
4. Make sure your Vite configuration correctly handles package imports

## License

[MIT License](LICENSE)

## Acknowledgments

- Special thanks to our bootcamp instructors for their guidance
- Product images used for demonstration purposes only
