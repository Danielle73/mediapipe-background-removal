# Live Background Remover

A real-time background removal application built with Next.js, React and Google's MediaPipe Selfie Segmentation.

The application uses a live camera feed to identify and isolate a person from their background, rendering the processed video onto an HTML canvas.

## Features

- Accesses a live camera feed using MediaPipe Camera Utils.
- Uses MediaPipe Selfie Segmentation to identify the foreground subject.
- Processes video frames in real time.
- Renders the segmentation output onto an HTML canvas.

## Technologies

- Next.js 14
- React 18
- JavaScript
- MediaPipe Selfie Segmentation
- MediaPipe Camera Utils
- Tailwind CSS

## Getting Started

### Prerequisites

- Node.js and npm
- A device with a camera
- Browser permission to access the camera

### Installation

Navigate to the project directory:

```bash
cd live-background-remover
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

Open [http://localhost:3000](http://localhost:3000) in your browser and allow camera access when prompted.

## How It Works

The application captures frames from the user's camera and processes them using MediaPipe Selfie Segmentation. The resulting segmentation mask is combined with the original image and rendered onto a canvas to isolate the foreground subject.

## Future Improvements

- Add options to replace the background with an image or colour.
- Improve camera controls and user experience.
- Add options to capture and save processed images.
