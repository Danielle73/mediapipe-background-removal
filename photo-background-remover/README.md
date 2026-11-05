# Photo Background Remover

A photo background removal application built with React, TypeScript and Google's MediaPipe Selfie Segmentation.

The application allows users to upload an image, identify the foreground subject and generate a processed image with the background removed.

## Features

- Upload images from your device.
- Preview the selected image before processing.
- Use MediaPipe Selfie Segmentation to identify the foreground subject.
- Process images using the HTML Canvas API.
- Display the processed image as a PNG.

## Technologies

- React 18
- TypeScript
- Vite 6
- MediaPipe Selfie Segmentation
- Three.js

## Getting Started

### Prerequisites

- Node.js and npm
- A modern web browser

### Installation

Navigate to the project directory:

```bash
cd photo-background-remover
```

Install the dependencies:

```bash
npm install
```

### Running the application

Start the development server:

```bash
npm run dev
```

Vite will provide a local URL in the terminal, usually [http://localhost:5173](http://localhost:5173).

Open this URL in your browser to use the application.

## How It Works

The application uses React state to manage the uploaded and processed images. When an image is selected, the FileReader API converts it into a data URL.

MediaPipe Selfie Segmentation then analyses the image and generates a segmentation mask. The HTML Canvas API combines the mask with the original image, producing a processed PNG that is displayed to the user.

## Future Improvements

- Add the ability to download processed images.
- Allow users to replace the background with a colour or image.
- Improve image upload and preview controls.
- Add support for processing multiple images.
