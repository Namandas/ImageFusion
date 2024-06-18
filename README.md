# ImageFusion: SaaS Image Manipulation Tool

[Live Demo](https://imagefusion-mocha.vercel.app)

ImageFusion is a powerful SaaS application designed to provide a range of image manipulation features using advanced AI algorithms. It leverages Cloudinary for image processing, Clerk for account management, and Stripe for handling payment transactions. The application is built with Next.js, MongoDB, and TypeScript, ensuring a robust and scalable platform.

## Features

ImageFusion offers the following image manipulation functionalities:

1. **Image Restore**: Restore old or damaged images to their original quality.
2. **Generative Fill**: Automatically fill in missing parts of an image using AI.
3. **Object Remove**: Remove unwanted objects from images seamlessly.
4. **Object Recolor**: Change the color of specific objects within an image.
5. **Background Remove**: Remove the background from images to isolate the main subject.

## Technology Stack

- **Frontend**: Next.js
- **Backend**: MongoDB
- **Programming Language**: TypeScript
- **Image Processing**: Cloudinary AI
- **Account Management**: Clerk
- **Payment Processing**: Stripe

## Usage

### Account Management

ImageFusion uses Clerk for managing user accounts. Users can sign up and log in securely to access their personalized dashboard and manage their image manipulation tasks.

### Credit System

ImageFusion operates on a credit system. Each user is allocated a set of free credits upon signing up. Once these credits are exhausted, additional credits can be purchased through Stripe. This system ensures that users pay only for the services they use.

### Image Manipulation

To use the image manipulation features, users can:

1. **Log in to their account.**
2. **Upload the image they want to manipulate.**
3. **Choose the desired feature from the left-hand panel:**
    - Image Restore
    - Generative Fill
    - Object Remove
    - Object Recolor
    - Background Remove
4. **Follow the on-screen instructions to apply the selected feature.**
5. **Download the transformed image.**

## Installation and Setup

To set up the ImageFusion application locally for development purposes, follow these steps:

1. **Clone the repository:**
   ```bash
   https://github.com/Namandas/ImageFusion/
2. **Navigate to the project directory:**
   ```bash
   cd Imagefusion
3. **Install the dependencies:**
   ```bash
   npm i
4. **Set up environment variables:**
   ```bash
    #NEXT
    NEXT_PUBLIC_SERVER_URL=
    NEXT_PUBLIC_CLERK_SIGN_IN_URL = /sign-in
    NEXT_PUBLIC_CLERK_SIGN_UP_URL = /sign-up
    NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL = / 
    NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL = /   
    #CLERK
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=
    WEBHOOK_SECRET=
    #MONGODB_
    MONGODB_URL=
   #CLOUDINARY
   NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
   CLOUDINARY_API_KEY=
   CLOUDINARY_API_SECRET=
   #STRIPE
   STRIPE_SECRET_KEY=
   STRIPE_WEBHOOK_SECRET=
   NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=

5. **Run the application:**
   ```bash
   npm run dev
6. **Open your browser and navigate to:**
   ```bash
   http://localhost:3000
