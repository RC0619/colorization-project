# AI Image Colorization Project

## Project Overview

This project explores AI-based image colorization using pretrained deep learning models. The aim is to convert grayscale images into plausible color images.

I reproduced and tested two pretrained models from the original Colorful Image Colorization project:

- **ECCV 2016**
- **SIGGRAPH 2017**

## My Contributions

- Cloned the original GitHub repository.
- Set up the Python environment and installed the dependencies.
- Ran the image colorization demo.
- Tested two pretrained models.
- Saved and compared the generated results.
- Documented the reproduction process.

I used pretrained models rather than training the models from scratch.

## Project Results

### ECCV 2016

![ECCV 2016 Result](saved_eccv16.png)

### SIGGRAPH 2017

![SIGGRAPH 2017 Result](saved_siggraph17.png)

Both models generate plausible color images from grayscale inputs. Their predictions may differ because they use different approaches.

## How to Reproduce

### Step 1: Clone the Repository

```bash
git clone https://github.com/RC0619/colorization-project.git
cd colorization-project
```

### Step 2: Install Dependencies

Use a compatible Python environment, then run:

```bash
pip install -r requirements.txt
```

### Step 3: Run Inference

```bash
python demo_release.py -i imgs/ansel_adams3.jpg
```

This runs the image colorization demo on an example image.

The required pretrained model weights must be available. See the original repository for model setup instructions.

## Challenges and Reflection

The main challenges were understanding the repository structure, configuring the Python environment, and learning how to run pretrained models.

This project helped me understand the basic workflow of AI inference, from preparing input images to generating and comparing outputs.

A limitation is that grayscale images do not contain their original color information, so the models predict plausible colors rather than guaranteed correct colors.

## Original Project and References

This reproduction is based on the original research and implementation by Richard Zhang and collaborators.

**Original GitHub Repository:** https://github.com/richzhang/colorization

**Research Papers:**

- Zhang, Isola, and Efros (2016). *Colorful Image Colorization*. ECCV.
- Zhang et al. (2017). *Real-Time User-Guided Image Colorization with Learned Deep Priors*. SIGGRAPH.

The original authors retain credit for the pretrained models and research.
