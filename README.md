# Video Analytics Pipeline with Dynamic Control

## Introduction

This repository hosts an application built to conduct video analysis in real-time. The application utilizes the GStreamer framework for video streaming, and Tkinter for creating an interactive GUI to control variables during runtime.

This software runs on a Jetson Xavier NX device, using the power of its GPU to accelerate the video processing tasks. The video analysis comprises of several stages, including segmentation, landmark detection, and edge detection. 

The application features an adaptive FPS strategy, adjusting to the camera's FPS and preventing frame buffering if the calculations cannot keep up with the camera's frame rate. This design allows for an optimized performance, enabling seamless video processing.

The software uses multiple models to perform video analytics tasks:

1. **Yunet** for edge detection. Our implementation is based on the OpenCV implementation. We extend our thanks to the original authors of Yunet for making their work available.

2. **DexiNed** for performing other types of edge detection. The original model was provided by the authors of DexiNed, whom we would like to acknowledge for their work.

3. A **landmark detection model** in Nvidia's Transfer Learning Toolkit (TLT) format, provided by Nvidia. We are grateful to Nvidia for providing this valuable resource.

## Credits

This project relies on the previous works of multiple authors. We would like to extend our gratitude to:

1. The original authors of the Yunet implementation in OpenCV.
2. The authors of the DexiNed model.
3. Nvidia for providing the landmark detection model in their Transfer Learning Toolkit (TLT) format.

## License

This project is licensed under the terms of the MIT license.

## Contact Information

For any queries, please feel free to reach out to the repository owner.
