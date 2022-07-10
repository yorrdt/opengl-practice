# opengl-practice

Improving practical skills in OpenGL

## IDE

Code::Blocks with MinGW

## Libraries

- GLFW
- GLEW
- GLM

**Building libraries (except GLM, because GLM is header only library) through CMake.**

## Linking to IDE

### Build options... -> Linker settings -> Link libraries:

- glew32
- glu32
- opengl32
- glfw3
- gdi32

**Must be in that order!**

![Illustration](https://github.com/yorrdt/opengl-practice/blob/main/illustrations/linker_settings-link_libraries.jpg)

### Build options... -> Search directories -> Compiler:

- "sources\include",
- "sources\include\GLEW",
- "sources\include\GLFW"

**Warning: relative path.**

![Illustration](https://github.com/yorrdt/opengl-practice/blob/main/illustrations/search_directories-compiler.jpg)

### Build options... -> Search directories -> Linker:

- "sources\lib",
- "sources\lib\GLEW",
- "sources\lib\GLFW"

**Warning: relative path.**

![Illustration](https://github.com/yorrdt/opengl-practice/blob/main/illustrations/search_directories-linker.jpg)

### Build options... -> Compiler settings -> #defines:

- GLEW_STATIC

![Illustration](https://github.com/yorrdt/opengl-practice/blob/main/illustrations/compiler_settings-defines.jpg)

## Build and run

![Illustration](https://github.com/yorrdt/opengl-practice/blob/main/illustrations/build_and_run.jpg)
