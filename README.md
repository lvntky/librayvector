# librayvector | Simple Vector Library

The librayvector is a lightweight single-header library for performing vector operations in C programming. It provides basic functionalities for working with 2D and 3D vectors, including addition, subtraction, dot product, cross product, normalization, and more. This library is suitable for C developers who need simple vector manipulation capabilities in their projects.

## Features

- Support for 2D and 3D vectors (`Vec2f` and `Vec3f`).
- Vector addition and subtraction.
- Vector dot product calculation.
- Vector cross product calculation (only for 3D vectors).
- Vector normalization.
- Convenience functions for vector initialization and printing.

## Usage

### Including the Library

To use the C Vector Library in your C project, include the `geometry.h` header file:

```c
#include "librayvector.h"
```

### Initializing Vectors
```c
Vec2f v2 = vec2f_init();
Vec3f v3 = vec3f_init();
```

### Performing Vector Operations
```c
Vec3f v1 = {1.0f, 2.0f, 3.0f};
Vec3f v2 = {4.0f, 5.0f, 6.0f};

// Vector addition
Vec3f result_add = vec3f_add(v1, v2);

// Vector subtraction
Vec3f result_sub = vec3f_subtract(v1, v2);

// Dot product
float dot_product = vec3f_dot(v1, v2);

// Cross product (only for 3D vectors)
Vec3f cross_product = vec3f_cross(v1, v2);

// Vector normalization
Vec3f normalized = vec3f_normalize(v1);
```

### Printing Vectors
```c
printf("Vector 2D: ");
vec2f_print(v2);

printf("Vector 3D: ");
vec3f_print(v3);
```

## License
This library is provided under the MIT License. You are free to use it in both open-source and closed-source projects.

## Contributions
Contributions and improvements to this library are welcome! If you find a bug or have a feature request, please open an issue or submit a pull request.

Happy coding!

