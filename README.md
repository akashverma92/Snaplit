# SNAPLIT – Full Stack AI-Powered Image Editor
🔗 **Live Demo:** [[https://snaplit-akash.vercel.app](https://snaplit-akash.vercel.app/)]

SNAPLIT is a modern, full-stack image editor built with **Next.js**, **Fabric.js**, and **ImageKit.io**, designed to provide both basic and advanced image editing features. It allows users to upload, crop, resize, and overlay images, with **AI-powered enhancements and transformations** for pro users. Additionally, users can fetch creative backgrounds from **Unsplash API** and apply them seamlessly.  

---

## Features

### **Basic Features (Free Users)**
- Upload images from local storage.
- Resize and crop images using ImageKit.io real-time URL-based transformations.
- Add text and image overlays on top of the base image using **Fabric.js**.
- Drag, rotate, and scale overlays interactively on the canvas.

### **Pro Features (Paid/Pro Users)**
- **AI Enhancements:** Improve image quality, upscale images, apply filters, and effects.
- **AI Transformations:** Generate creative variations, remove or replace backgrounds.
- Background removal and editing powered by **ImageKit API**.
- Apply backgrounds from **Unsplash API** by searching for keywords (e.g., "road", "nature").

### **Additional Features**
- Real-time image transformation and delivery without storing multiple versions.
- Clean, responsive, and interactive user interface.
- Supports dynamic text styling and positioning on images.

---

## Tech Stack

- **Frontend & Backend:** [Next.js](https://nextjs.org/) (React-based framework)
- **Canvas & Image Manipulation:** [Fabric.js](http://fabricjs.com/)
- **Image Storage & Transformations:** [ImageKit.io](https://imagekit.io/)
- **Background Images:** [Unsplash API](https://unsplash.com/developers)
- **Styling:** CSS / Tailwind CSS (if used)

---

## Project Architecture

1. **Frontend (Next.js + Fabric.js)**
   - Handles user interactions: uploading images, adding overlays, drawing on canvas.
   - Sends transformation requests to ImageKit via URL parameters.

2. **Image Transformations (ImageKit.io)**
   - Resizing, cropping, filters, AI enhancements, background removal.
   - Generates transformed images in real-time.

3. **Background Integration (Unsplash API)**
   - Fetch images based on user search.
   - Apply selected image as a new background on the canvas.

---

## Getting Started

### Prerequisites
- Node.js >= 16
- NPM or Yarn
- ImageKit account (for API key and URL endpoint)
- Unsplash API access key (optional, for background search feature)

### Installation
```bash
# Clone the repository
git clone https://github.com/akashverma92/snaplit.git

# Navigate to the project folder
cd snaplit

# Install dependencies
npm install

# Run the development server
npm run dev
