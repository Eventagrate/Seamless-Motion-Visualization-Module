

# Seamless-Motion-Visualization-Module
## About

The Bone Positioning Tracker is 8th Wall Module application that allows users to track body movements in real-time and receive valuable feedback on bone positions and actions. This feedback can be utilized to create customized body positions, enabling users to embrace frictionless movement expression. The Module was created for the 8th wall Community Module challenge. https://itch.io/jam/8th-wall-modules-challenge

Module Import Page: https://www.8thwall.com/mimicdigital/modules/pose-detection



## Getting Started

### Technical Stack

The Bone Positioning Tracker is built using the following technologies:

- **aframe + three.js**: This project utilizes the aframe and three.js libraries for creating the interactive 3D scene.
- **TensorFlow.js**: The application employs TensorFlow.js for live pose detection.
- **Posenet**: Posenet, a deep learning model provided by TensorFlow, is used for accurate pose detection.

### Prerequisites

Before using the Bone Positioning Tracker, you need to add the following dependencies (script tags) to the head.html file of your project:

```html
<script crossorigin="anonymous" src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
<script crossorigin="anonymous" src="https://cdn.jsdelivr.net/npm/@tensorflow-models/pose-detection"></script>
<script crossorigin="anonymous" src="https://cdn.jsdelivr.net/npm/@tensorflow-models/posenet@2.2.2/dist/posenet.min.js"></script>
```

### Adding a Module

To add a module, navigate to the "Modules" tab and select the desired module to include in your project.

### Creating a Scene

To create a scene for the Bone Positioning Tracker, use the following parameters:

```html
<a-scene
  xrextras-tap-recenter
  landing-page
  xrextras-loading
  xrextras-runtime-error
  xrextras-pause-on-hidden
  xrface="mirroredDisplay: true; cameraDirection: front; allowedDevices: any;"
>
```

Within this scene, create an empty entity and add the 'pose-detection' component to enable seamless motion visualization:

```html
<a-entity pose-detection></a-plane>
```

## Troubleshooting

If you encounter any issues while using the Bone Positioning Tracker, consider the following steps:

1. Ensure that all the dependencies are properly added to the head.html file.
2. Check if your system meets the specified requirements for the application to function correctly.
3. For any runtime errors or issues related to pose detection, refer to the TensorFlow.js and Posenet documentation.
