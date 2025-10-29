# ❗️❗️❗️ Canceled, Sorry. ❗️❗️❗️

--------

<!-- Language switch -->
[🇩🇪 Deutsch](DEUTSCH.md) | [🇺🇸 English](README.md)

## AI-powered 3D Engine for Point Clouds & VR

_A groundbreaking solution for generating, interpreting, and editing 3D point cloud data for design, manufacturing, creative 3D applications, the gaming industry, and VR visualization – flexible, scalable, and intuitive._

## 🚧 Problem Statement

🤖 AI systems struggle to analyze, interpret, and edit 3D structures such as B-Rep, NURBS, meshes, CSG, SDF, voxels, and polygonal networks, as these traditional representations are often too complex, memory-intensive, or inefficient for deep learning models.

## 🛠️ Solution

Modern AI technologies are already successfully used in areas like text and image recognition.

With the next generation, AI is now entering a particularly promising field: the processing of **point clouds**. These offer a **forward-looking**, **flexible**, and **highly scalable** foundation for AI-powered analysis, object recognition, and further processing.

## ✨ Why Are Point Clouds Better?

Point clouds are **lightweight**, **transparent**, **flexible**, **highly scalable**, and **particularly AI-friendly**. They enable fast, precise detection of geometric features and can be processed **efficiently** using modern deep learning architectures.

In contrast, traditional CAD systems like SolidWorks or Autodesk still primarily rely on B-Rep and NURBS – structures that are significantly harder to access for AI.

Comparison: A technical drawing on A4 paper appears lightweight – easily readable at about 50 KB. However, it may contain complex geometries which, in precise digital CAD representation, can quickly reach 100 MB or more depending on the chosen format. Therefore, it's beneficial to convert such drawings into a lightweight point cloud structure – reducible to around 10 KB depending on the chosen option.

## 💡 My Innovative Approach

Each point is enriched with precise geometric information – e.g., distances to defined reference points, spatial orientations, and references to relevant parameters and variables – to enable better AI interpretation. This provides a significant advantage in analysis and downstream processing.

The geometric information is inspired by similar concepts from B-Rep and NURBS, enabling lossless transfer to traditional 3D modeling systems such as Parasolid.

Point clouds should serve as the **primary data basis** for AI applications, while B-Rep and NURBS should be **used complementarily** – e.g., for export, tolerance definition, use in CAD core systems like Parasolid, or integration into manufacturing workflows.

## 🧱 Rethinking the Classic 3D Surface

For example, a single click is enough to instantly update a 3D surface – like in a real CAD model with B-Rep/NURBS.

After each change, the system automatically switches back to the point cloud structure to allow further AI-supported editing steps. A middleware interprets inputs via mouse, keyboard, or gestures – unlike traditional CAD systems.

The AI "understands" point clouds – while humans perceive 3D surfaces better visually. This interplay enables intuitive operation with maximum AI support in the background.

Combining point clouds with B-Rep/NURBS in real-time processing is technically possible but significantly more complex and will be pursued later. These are fundamentally different data models that must be interpreted separately. Especially with B-Rep/NURBS, model errors can lead to crashes – whereas point clouds allow stable processing even if incomplete.

## 🔧 Functionality

The AI can precisely analyze 3D point cloud data – for example:
"The part contains three M16 threaded holes, each 25mm deep, five flat surfaces, 15 edges, ten holes, and three freeform surfaces. A thin-walled structure is present. Additional metadata includes tolerance values, material, color, purpose, manufacturing effort, etc."

Even complex components or assemblies are reliably detected and analyzed.
If the AI cannot clearly classify an unknown component, it asks the user for its intended purpose – and uses this information for continual learning.

Moreover, the AI can reconstruct incomplete parts and generate multiple (e.g., ten) plausible design suggestions.

It can also convert both technical drawings and simple text descriptions such as:
"Cylinder D20×L100 with through hole d3, all edges rounded R1"
into corresponding point cloud structures.

It can even generate complete 3D models based on voice commands, e.g.:
"Create a car."
Geometry can then be modified:
"Change the car to a Ferrari."
Or more advanced:
"Disassemble the car into components."

The AI can also generate point-cloud-based text inside point cloud representations.

Additionally, the AI understands gestures – including sign language – using point cloud data alone (no mesh or polygon net).

## 🗂️ New Data Format

The planned format **.pbin** (if available) is designed specifically for AI-powered applications in CAD, digital manufacturing, 3D design, and gaming. Unlike classic formats like `.stl` or `.step`, which contain limited information (e.g., no tolerances), `.pbin` includes not only geometric point data but also rich additional data – as described below:

- Tolerance data per technical standards – e.g., between points, fully embedded
- Multiple point types – visible, invisible, human, ghost, zombie
- Technical metadata such as material, surface roughness, thermal/surface treatment
- Layer thickness and allowances for coatings or special manufacturing
- Manufacturing hints and feature tags to mark critical areas – AI-readable
- Extendable extra data for animation, material effects, or game engines – with note: More info increases memory need, but bitmasks are used

**Goal:** A lightweight, future-proof, AI-compatible exchange format, usable in digital manufacturing, 3D studios, and game development.

## 🔬 Proof of Concept

Relevant reference projects:

- [learning3d – Modern 3D methods with PyTorch](https://github.com/vinits5/learning3d)
- [VIPL-SLP / PointLSTM – Gesture recognition from point clouds](https://github.com/VIPL-SLP/pointlstm-gesture-recognition-pytorch)
- [Deep Learning on Point Clouds – Overview of current models (PointNet, KPConv, etc.)](https://github.com/PointCloudYC/Deep-Learning-On-Point-Clouds)

These serve as the **technological foundation and inspiration** for our AI backend – especially in gesture recognition, object classification, and geometry analysis.

Experiments are conducted using:

**Deep Learning Frameworks**
- PyTorch, PyTorch Lightning
- SimCLR, MoCo, BYOL (SSL)
- TensorFlow, Keras
- MXNet, Caffe, JAX, Theano, Chainer
- ONNX

**Computer Vision & 3D**
- DINO, DINOv2, SimCLR, Barlow Twins
- PointContrast, SparseConv Scene Context
- OpenCV, Tesseract OCR

**3D & CAD Engines/Libraries**
- OpenCASCADE, Open3D, PCL, Trimesh, MeshLab
- GLSL, CUDA shaders for Vulkan/Unity/Unreal

**Point Clouds & Geometry**
- PointNet, DGCNN, KPConv, Point Transformer
- SparseConv3D, PCNN, VoxelNet, DenseNet

**3D Reconstruction & Representation**
- Pix2Vox, NeRF, IM-NET, MeshCNN
- 3D-GAN, SDF, 2D→3D networks

**Image Processing & Object Detection**
- ResNet, CNN, RNN/LSTM, GAN/VAE
- YOLO, ViT, DeepLab, Mask R-CNN

**Datasets & Feature Detection**
- ShapeNet, ABC Dataset
- Feature detection for holes, grooves, freeform surfaces

## 🌀 Conclusion

Without AI, point clouds would be largely useless in the CAD world – unlike classic CAD geometries, they cannot be parametrically controlled.

In other words: Without AI, point clouds remain "points in space" – without context, structure, or actionable meaning. Only AI gives them semantic depth, making them truly usable in design.

With AI, point clouds become a powerful tool enabling new possibilities in design, analysis, simulation, and automation.

## 🎯 Goal

Develop a powerful 3D engine that:
- enables interactive editing of point clouds via mouse or gestures,
- acts as an AI-supported modeling platform for point clouds,
- uses modern rendering technologies like Vulkan or WebGPU,
- automatically converts 2D drawings into 3D models,
- is based on modern AI for pattern recognition and geometry reconstruction,
- allows intuitive input of basic shapes (lines, circles) via gesture control (stereo dual camera), mouse, or keyboard – like CAD software, but consistently point-cloud-based and AI-powered.

**Target audience:** mechanical engineering and manufacturing industries, especially CNC.
