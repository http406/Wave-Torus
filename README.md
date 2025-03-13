# Wave-Torus

### What is a Wave Torus?

A **Wave Torus** is a variation of a standard torus (a doughnut-shaped surface) that incorporates a wave-like modulation along its surface. This modulation creates a rippled or undulating effect, giving the torus a more complex and visually interesting shape. The Wave Torus can be used in various fields such as computer graphics, architectural design, and artistic visualization to create intricate and dynamic 3D models.

### Equation Explanation

The equation used to define the Wave Torus in the code is a parametric equation that describes the coordinates \((x, y, z)\) of points on the surface of the torus. Here's the equation broken down:

![Image](https://github.com/user-attachments/assets/546bae73-96a0-4241-9c34-be8b14d310fc)

Where:

![Image](https://github.com/user-attachments/assets/4a6cd565-e9a5-4022-aeba-0ac067eb061b)

### Parameters in the Code

In the provided code, the parameters are set as follows:
- \(R = 6\)
- \(r = 0.8\)
- \(a = 2.2\)
- \(n = 8\)

### Detailed Explanation of the Equation

1. **Major Radius (\(R\))**: This is the distance from the center of the torus to the center of the tube. It defines the overall size of the torus.

2. **Minor Radius (\(r\))**: This is the radius of the tube itself. It defines the thickness of the torus.

3. **Wave Modulation (\(a \sin(n u)\))**: This term introduces the wave-like modulation to the torus. The amplitude \(a\) controls the height of the waves, and the frequency \(n\) controls how many waves are present around the torus.

4. **Parametric Angles (\(u\) and \(v\))**: These angles parameterize the surface of the torus. The angle \(u\) varies around the major radius, and the angle \(v\) varies around the minor radius.

### How the Equation Works

- **\(x\) and \(y\) Coordinates**: These coordinates are calculated by first determining the distance from the center of the torus to a point on the tube, which is \(R + (r + a sin(n u)) cos(v)\). This distance is then multiplied by (cos(u)\) and (sin(u)\) to get the \(x\) and \(y\) coordinates, respectively.
  
- **\(z\) Coordinate**: This coordinate is determined by the height of the point on the tube, which is \((r + a sin(n u)) sin(v)\).

### Visualization

When you plot these equations, you get a torus with a wave-like pattern along its surface. The wave modulation creates a visually appealing effect, making the torus look like it has ripples or waves moving around it.

### Footnote 

In the provided JavaScript code using Three.js, the Wave Torus is created by generating vertices based on the above equations. These vertices are then used to create a 3D mesh that can be rendered and animated in a WebGL scene. The rainbow color effect and the space background with glittering stars further enhance the visual appeal of the Wave Torus.

By understanding the equation and its parameters, you can modify the shape and appearance of the Wave Torus to suit different visual and design needs.
