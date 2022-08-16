# Modular-CMake-Project
A CMake project that allows you to pick and choose compile-time modules.

The project consist of a library and an executable. The library further consists the core library, a header library, and the available modules. The modules are static libraries that link to the header library to facilitate communication between the modules and the library. The engine then links to to header library and modules. This project provides CMake functions that make it easy to declare and use modules. The executable links to the library as any executable would without need to interact with the modules. This project uses the example of a game engine with an editor (the executable), an engine (the library), and an engine extension (the module). This template makes use of CMake's `configure_file` function to generate a source file that initializes and deinitializes the modules.
