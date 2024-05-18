## Edge-based Line Average (ELA) Algorithm

The **Edge-based Line Average (ELA) Algorithm** relies on using linear interpolation to find the appropriate pixel value by applying fuzzy rules to its fuzzy variables, which represent the output image.

### Input
The input consists of the pixels surrounding the current pixel. Each surrounding pixel is represented as a fuzzy variable with a fuzzy set characterized by a Gaussian membership function level, which represents the intensity of the pixel (the amount of density). There are 3 levels:
1. **Small**
2. **Medium**
3. **Big**

### Output
The output is the density of the current pixel.

### Algorithm
ELA is an algorithm that performs linear interpolation for the pixels based on rules, with its input being the neighboring pixels.

- The rules aim to preserve the edges and their directions by predicting the pixel value using the known neighboring pixels.
- It also maintains color consistency in areas of the image with small color variations by predicting a pixel with an appropriate color gradient.
