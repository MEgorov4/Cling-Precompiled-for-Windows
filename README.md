# Cling for Windows with Visual Studio 2019 SDK

This repository contains a precompiled version of the interactive C++ interpreter `cling` for Windows, configured to work with Microsoft Visual Studio 2019 and Windows 10 SDK.
`VS19 16.11.34 tested`

## Installation

Follow these steps to use `cling` in your development environment:

### Step 1: Install Visual Studio 2019

Install Visual Studio 2019 with the C++ development component and Windows 10 SDK. This is necessary for the correct operation of `cling` and ClingVS19EnvLauncher.

- [Download Visual Studio 2019](https://visualstudio.microsoft.com/vs/older-downloads/)

During the installation process, select the "Desktop development with C++" workload to install the C++ compiler and necessary tools.

### Step 2: Add `cling.exe` to PATH

Add the path to `cling.exe` to the `PATH` environment variable to make `cling` accessible from the command line anywhere.

1. Determine the path to `cling.exe` on your system.
2. Open "System Properties" > "Advanced system settings" > "Environment Variables".
3. Find the `Path` variable in the "System variables" section and select "Edit".
4. Add the path to `cling.exe` at the end of the list.

### Step 3: Add `vcvarsall.bat` to PATH

Similarly, add the path to `vcvarsall.bat` to the `PATH` environment variable. This ensures the correct environment setup for `cling`.

`vcvarsall.bat` is typically located at:
C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\VC\Auxiliary\Build\vcvarsall.bat

### Step 4: Run ClingVS19EnvLauncher

After configuring `PATH`, use `ClingVS19EnvLauncher` to launch `cling` with the correct environment for Visual Studio 2019 and Windows 10 SDK. `ClingVS19EnvLauncher` will automatically set the necessary environment variables.

## Usage

To run `cling`:
ClingVS19EnvLauncher.exe

Now you can use the interactive C++ interpreter `cling` to execute C++ code on the fly.

---

