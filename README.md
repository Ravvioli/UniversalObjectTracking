# Universal Object Tracking Pipeline


This notebook runs a real-time object detection and tracking pipeline inside Google Colab using your webcam. 

It uses the nvidia/LocateAnything-3B vision-language model to locate items directly on your hardware.

## How to Run
1) Verify GPU Hardware: Ensure your Colab runtime is set to a T4 GPU (Runtime > Change runtime type > T4 GPU).

2) Execute Cell 1 & 2: Install dependencies and load the model weights into memory.

3) Run Cell 3: Start the embedded web application widget.

## Track Targets: 
Type what you want to find into the text input box (e.g., cup, a black cup, foam), then click Start Tracking. Leaving the box blank defaults to tracking human faces and eyes.

## Workflow Layout
Cell 1 (Setup): Installs required packages. Run once per session.

Cell 2 (Model initialization): Loads the 3B parameter model into your GPU VRAM. Run once.

Cell 3 (Interactive Interface): Contains the Python-to-JavaScript bridge and the camera interface. Run this cell whenever you want to reset or update the web application tracking view.
