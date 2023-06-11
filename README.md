# AI Light Show Instalation

## Introduction

This repository hosts the underlying structure for an AI Light Show. The AI workflow run on a NVIDIA Jetson Orin with Jetpack 5.0.2. The light control workflow may run on any MAC OS or windows system. The AI workflows require the Python 3.8, GStreamer, TensorRT, OpenCV with CUDA support. The light control workflows are handeled in touchdesigner.

![AI Light Show Example](example.gif)

The AI workflow uses three open-source Neural Netowrks:

**DexiNed:** This model is a product of research by Xiaofeng Liu, Joost van de Weijer, and Andrew D. Bagdanov from the Computer Vision Center, Universitat Autònoma de Barcelona. DexiNed is designed for edge detection in images and uses a unique multi-task learning approach to capture and unify the informative features at different scales.

**YuNet:** Developed by the team at Vision Perception and Intelligence Group of Baidu Research, Yunet is a state-of-the-art model designed for real-time holistic edge detection, producing high-quality edge maps with improved accuracy and efficiency.

**Nvidia's TLT Landmark Detection Model:** This model is provided by Nvidia, a leading company in AI and Deep Learning technologies. It's designed for precise landmark detection in images, useful for tasks like facial feature detection, object detection, and more, and is optimized for efficient deployment on Nvidia's GPU architectures.

The output of the AI workflow is streamed over network to another device running touchdesigner. Touchdesigner controls the light machines to create a dynamic, intercative, AI-driven light show.

## Credits

This project relies on the previous works of multiple authors. We would like to extend our gratitude to:

1. The original authors of the Yunet implementation in OpenCV.
2. The authors of the DexiNed model.
3. Nvidia for providing the landmark detection model in their Transfer Learning Toolkit (TLT) format.

## License

This project is licensed under the terms of the MIT license.

## Contact Information

For any queries, please feel free to reach out to the repository owner.
