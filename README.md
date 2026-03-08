# Morphological Image Operations

Digital Image Processing project exploring morphological operations used for image structure analysis and noise removal.

The project implements several fundamental morphological operations from scratch, including erosion, dilation, opening, and closing, and demonstrates their effects on different images.

---

# Project Structure

```
morphological-image-operations/
│
├── notebooks/
│   └── morphological_operations.ipynb
│
├── data/
│   └── all example images used in the project can be found here
│
└── README.md
```

---

# Project Overview

Morphological image processing is a set of operations that process images based on shapes and structures.

These operations are commonly used for:

- removing noise
- separating objects
- filling small gaps
- refining segmentation results

In this project, several morphological operations are implemented manually and applied to different images to observe their effects.

---

# Implemented Operations

The following morphological operations are implemented.

---

## 1. Erosion

Erosion shrinks bright regions in a binary or grayscale image.

Each pixel is replaced by the minimum value within its neighbourhood defined by a structuring element.

Effects of erosion include:

- shrinking objects
- removing small noise pixels
- separating connected objects

---

## 2. Dilation

Dilation expands bright regions in an image.

Each pixel is replaced by the maximum value within its neighbourhood.

Effects of dilation include:

- expanding objects
- filling small gaps
- connecting nearby structures

---

## 3. Opening

Opening is a combination of erosion followed by dilation.

```
Opening = Erosion → Dilation
```

This operation is useful for:

- removing small objects
- smoothing object boundaries
- preserving larger structures

---

## 4. Closing

Closing is the opposite sequence of operations:

```
Closing = Dilation → Erosion
```

Closing is commonly used for:

- filling small holes inside objects
- closing small gaps
- connecting nearby regions

---

# Results and Evaluation

The operations are tested on different images in order to evaluate their behaviour.

Observations include:

- Erosion reduces object size and removes small noise.
- Dilation expands object boundaries and fills gaps.
- Opening effectively removes small artifacts.
- Closing fills small holes and smooths boundaries.

These operations are fundamental tools in image preprocessing and segmentation tasks.

---

# Technologies Used

- Python
- NumPy
- OpenCV
- Matplotlib
- Jupyter Notebook

---

# Running the Project

Clone the repository:

```
git clone <repository-url>
```

Install dependencies:

```
pip install numpy opencv-python matplotlib
```

Launch Jupyter Notebook:

```
jupyter notebook
```

Open and run:

```
notebooks/morphological_operations.ipynb
```

---

# Concepts Demonstrated

This project demonstrates several key concepts in digital image processing:

- morphological image processing
- erosion and dilation
- opening and closing operations
- structuring elements
- image preprocessing
