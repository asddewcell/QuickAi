# Quick AI - PERN Stack AI SaaS App

Quick AI is a comprehensive, full-stack AI-powered Software as a Service (SaaS) web application I built using the PERN (PostgreSQL, Express.js, React.js, Node.js) stack. This project allows users to leverage a variety of AI tools for content creation, image manipulation, and professional development. The application also features a robust subscription system to manage access to premium features.

[Live Demo Link: https://quick-ai-five-tau.vercel.app/](https://quick-ai-five-tau.vercel.app/)

-----

### ✨ Features

#### For Users 🙋‍♂️

  * **Authentication**: Secure user sign-up and login powered by **Clerk**, supporting both social media accounts and traditional email/password registration.
  * **AI-Powered Tools**:
      * **📝 Article Generator**: Generate articles on any given topic with selectable length options.
      * **✍️ Blog Title Generator**: Get suggestions for blog titles based on keywords.
      * **🖼️ Image Generator**: Create images from textual descriptions with different style choices.
      * **✂️ Background Remover**: Upload an image to automatically remove its background.
      * **🚫 Object Remover**: Remove specific objects from an image by describing them.
      * **📄 Résumé Analyzer**: Upload a résumé to receive a detailed analysis, including strengths, weaknesses, and areas for improvement.
  * **Subscription Management**: Easily upgrade from a free to a premium plan to unlock all AI features.
  * **Community Feed**: View and "like" AI-generated images shared by other users in the community.
  * **Creation History**: A dashboard to view all your past creations and manage your account.

#### For Admins 👨‍💻

  * **User Management**: Manage users and authentication through the Clerk dashboard.
  * **Database Management**: Monitor and manage application data via the Neon serverless Postgres dashboard.
  * **Payment & Subscription Oversight**: Track subscriptions and payments through the integrated billing system.

-----

### 🛠️ Tech Stack

  * **Frontend**: React.js, Vite, Tailwind CSS, Clerk, React Router
  * **Backend**: Node.js, Express.js
  * **Database**: PostgreSQL (Neon)
  * **Services**:
      * **Clerk**: User authentication and management.
      * **Gemini API**: For content generation.
      * **ClipDrop API**: For image manipulation.
      * **Cloudinary**: For image storage and delivery.
  * **Deployment**: Vercel

-----

### 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

#### Prerequisites

  * Node.js (v18 or later recommended)
  * npm or yarn
  * A code editor like VS Code

#### Setup and Installation

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/quick-ai.git
    cd quick-ai
    ```

2.  **Setup the Backend (`/server`)**:

      * Navigate to the `server` directory: `cd server`
      * Install dependencies: `npm install`
      * Create a `.env` file in the `/server` root and add the following variables with your credentials:
        ```env
        DATABASE_URL='your_postgresql_connection_string'
        CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
        CLERK_SECRET_KEY=your_clerk_secret_key
        GEMINI_API_KEY=your_gemini_api_key
        CLIPDROP_API_KEY=your_clipdrop_api_key
        CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
        CLOUDINARY_API_KEY=your_cloudinary_api_key
        CLOUDINARY_API_SECRET=your_cloudinary_api_secret
        ```
      * Start the server: `npm run server`

3.  **Setup the Frontend (`/client`)**:

      * Navigate to the `client` directory from the root folder: `cd client`
      * Install dependencies: `npm install`
      * Create a `.env` file in the `/client` root and add the following:
        ```env
        VITE_CLERK_PUBLISHABLE_KEY=your_vite_clerk_publishable_key
        VITE_BASE_URL=http://localhost:3000
        ```
      * Start the client development server: `npm run dev`
      * Open your browser and navigate to the local URL provided (e.g., `http://localhost:5173`).
