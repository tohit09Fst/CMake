# Building a Project Using CMake

## Create a “Hello, World!” Project

This repository demonstrates how to build a simple "Hello, World!" program using CMake.

### Step 1: Create the C Program (`main.c`)

First, create a simple C program that prints "Hello, World!" to the console.

```c
#include <stdio.h>

int main() {
    printf("Hello, World\n");
    return 0;
}
```

### Step 2: Create the CMake Configuration (CMakeLists.txt)

```c
cmake_minimum_required(VERSION 3.10)
project(HelloWorld)

add_executable(hello main.c)

```

### Step 3: Build the Project

Follow these steps to configure and build your project:

##### 1. Navigate to the Project Directory:

Open a terminal and navigate to the root directory of your project where CMakeLists.txt is located.

##### 2. Run CMake to Generate Makefiles:

Run the following command to configure the project and generate Makefiles.

```c
cmake .
```
##### 3. Build the Project:

Use make to compile the project and create the executable:

```c
make
```
##### 4. Run the Executable:

After building, run the executable with the following command:

```c
./hello
```
###### You should see the output:
```c
Hello, World!
```
