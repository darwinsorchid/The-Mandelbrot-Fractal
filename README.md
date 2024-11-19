# Visualizing the Mandelbrot Fractal
[> The Mandelbrot Fractal Streamlit App](https://mandelbrot-fractal.streamlit.app/)

## Description
The Mandelbrot set is a famous fractal defined in the complex plane, named after mathematician Benoit Mandelbrot. It's generated by iterating a simple mathematical formula:

$$
z_{n+1} = z_n^2 + c
$$

where $z$ and $c$ are complex numbers. The iteration starts with $z_0 = 0$ and $c$ varies over the complex plane.


**Key Features:**

- Escape Time: The color of each point $c$ is determined by how quickly the iterated values $z_n$ escape to infinity (if they do).
Points that remain bounded (do not escape) belong to the Mandelbrot set and are typically colored black.
- Boundary Complexity: The boundary of the Mandelbrot set exhibits intricate and self-similar structures, revealing more detail as you zoom in.
- Fractal Nature: It demonstrates the key properties of fractals, including self-similarity and infinite complexity.


**Visualization:**

The set is typically visualized on a 2D plane where the x-axis represents the real part of $c$ and the y-axis represents the imaginary part. 
Different colors are assigned to points based on their escape time, resulting in different visual patterns.
Part of the Streamlit app are sidebar slider widgets to adjust the following parameters:
* Maximum number of iterations
* Image resolution
* Zoom factor
* Zoom center on real axis
* Zoom center on imaginary axis 


## Libraries

- `numpy`
- `matplotlib`
- `streamlit`


## Instructions

To run the Streamlit app and render the Mandelbrot plot, use the following command:

```bash
streamlit run Mandelbrot.py
