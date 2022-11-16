# [🧮Rubik's Cube Face Detection Model🚦](https://github.com/Hemant-Mulchandani/Rubiks-Cube-Face-Detection-Model)

* A deep learning object detection model built using SSD ResNet101 V1 FPN 640x640 in conjunction with TensorFlow object detection API. 

* Trained on a custom dataset (300+ images) for 10 different labels, the model detects tile colors on Rubik's cube face with **98-100% accuracy** and only **0.2 total loss.**

<p align="center">
  <img src="https://user-images.githubusercontent.com/89768465/194771951-de426a39-4a8e-46e9-a167-9c3bd672f39b.gif">
</p>

<h2>Motivation<span style='font-size:100px;'>&#127775;</span></h2>	

The scrambles are so varying and there are such a wide variety of events, that unless you get bored with the actual solving, you will never find yourself repeating an entire solution. Considering that there are **43,252,003,274,489,856,000** possible solvable states for the **3x3 Rubik's cube** alone, over **43 quintillion**, a number that significantly increases even just to the 4x4 cube, there are still only a small number of scrambles that have actually been solved.

## Mystery 🕵🏻

The mystery of the Magic's Cube consists in its simplicity and yet unsolvability. It's a very simple toy, everybody can understand what is the goal at the first time they hold it in their hands and it's still almost impossible to solve for a human being because you should foresee too many steps while solving it. When the puzzle was invented it took one month to solve it for the very first time. They weren't even sure that it was solvable until that point.

Mathematicians were analyzing the puzzle trying to solve its secrets. Various Rubik's Cube solver robots have been built to solve the Cube in a blink of an eye, and computer programs are searching for the optimal solution. Using the supercomputers of Google scientists have proved that any Rubik's Cube can be solved in **maximum 20 steps** from any random starting position. This is called the **God's Number.**

## Features :gem:
* Trained on a custom dataset (300+ images) for 10 different labels.
* The model detects tile colors on Rubik's cube face with **98-100% accuracy** and only **0.2 total loss.**

# Installation :package:

1. Clone the repo

```bash
   $ git clone https://github.com/Hemant-Mulchandani/Rubiks-Cube-Face-Detection-Model.git
```

2. Install dependencies

* Install dependencies like TensorFlow Object Detection API, COCO API, Protobuf, etc. required for this project from this [Installation Guide](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html).
```bash
   1. Python Verion: 3.7x
   2. TensorFlow Version: 2.9.1
   3. Protobuf: 3.15.8
   4. CUDA Toolkit: 11.3.1
   5. CUDNN: 8.2.1
```

 
  
  
<p align="center">
<img src="https://user-images.githubusercontent.com/89768465/194772094-c56c292f-c245-47c1-8d46-9b4c9305afb0.gif">
</p>
<p align="center">
<img src="https://user-images.githubusercontent.com/89768465/194772007-948fac47-29b7-45e9-906f-61e4201c2f99.gif">
</p>
