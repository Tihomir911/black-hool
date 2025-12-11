# KERR BLACK HOLE - Black Hole Visualizer

![System Requirements](https://img.shields.io/badge/System_Requirements-Windows-blue)
![Language](https://img.shields.io/badge/Language-C++17-red)
![Library](https://img.shields.io/badge/Library-SDL2-green)

## 📌 Project Description

This project is a highly optimized simulator of a rotating Kerr black hole with real-time visualization. The program models physical effects:
- Gravitational lensing of light
- Accretion disk with turbulence and hot spots
- Long photon trajectories around the black hole
- Frame-dragging effect (Lense-Thirring effect)

## 🚀 Features

- **Super-optimized rendering** - 320×180 resolution with upscaling to 1280×720
- **Stabilized Kerr metric** - no chaotic behavior
- **Interactive controls** - free camera movement around the black hole
- **Dynamic accretion disk** - with rotation, turbulence, and hot spots
- **Photon trajectories** - visualization of light paths around the black hole
- **Configurable parameters** - mass, spin, visibility of elements

## 📋 System Requirements

- **OS**: Windows 7/8/10/11 (64-bit)
- **CPU**: 2+ cores, 2.0+ GHz
- **RAM**: 4+ GB
- **GPU**: OpenGL 3.3+ support
- **Storage**: 50 MB

## ⚙️ Installation and Launch

### Option 1: Running Pre-built EXE
1. Download the release archive
2. Extract to any folder
3. Run `blackhole_final.exe`
4. Accept the CPU load warning
5. Configure parameters in the console menu

### Option 2: Building from Source (Visual Studio)

#### Step 1: Environment Setup
1. Install **Visual Studio 2019+** with C++17 support
2. Download **SDL2 development library** (SDL2-devel-2.x.x-VC.zip)
3. Create an empty Visual Studio project (Console Application)

#### Step 2: Project Configuration
1. Copy `blackhole_final_optimized.cpp` to the project
2. In project properties set:
   - **Configuration**: All Configurations
   - **C/C++ → General → Additional Include Directories**:
     ```
     <path_to_SDL2>\include
     ```
   - **Linker → General → Additional Library Directories**:
     ```
     <path_to_SDL2>\lib\x64
     ```
   - **Linker → Input → Additional Dependencies**:
     ```
     SDL2.lib;SDL2main.lib;Shell32.lib;user32.lib;gdi32.lib;winmm.lib
     ```

#### Step 3: Copying DLL
1. Copy `SDL2.dll` from `SDL2\lib\x64\` to the executable folder
2. Or add the DLL path to the PATH environment variable

#### Step 4: Building
1. Select **Release** configuration, **x64** platform
2. Build the project (Ctrl+Shift+B)
3. Run the resulting EXE file

## 🎮 In-Simulation Controls

### Camera Control:
- **W/S** - move forward/backward
- **A/D** - move left/right  
- **Q/E** - move up/down
- **Right mouse button + drag** - rotate camera
- **Mouse wheel** - zoom in/out

### Black Hole Interaction:
- **Left mouse click** - launch photon from camera to click point
- **Space** - launch photon straight forward from camera
- **P** - delete all photons

### System Commands:
- **R** - restart simulation with current parameters
- **ESC** - exit program

## ⚙️ Parameter Configuration

Upon launch, a console menu opens with parameters:

1. **Black hole mass** (0.5-20) - determines event horizon size
2. **Black hole spin** (-0.99 to 0.99) - rotation speed
3. **Initial camera distance** - observer position
4. **Show accretion disk** - enable/disable disk
5. **Show photons** - visualize light trajectories
6. **Render resolution** - fixed for stability

## 📊 Technical Features

### Optimizations:
- Low internal resolution (320×180)
- Skip every 3rd pixel during rendering
- Thread pool for computations
- Static memory allocation
- Optimized mathematical operations

### Physical Model:
- Kerr metric with spin parameter a = 0.99
- Stabilized geodesic equations
- Realistic accretion disk with temperature gradient
- Doppler effect for rotating matter
- Gravitational redshift

## 🗂️ Code Structure

```
blackhole_final_optimized.cpp
├── Vector mathematics (optimized)
├── KerrMetric class (Kerr metric)
├── Photon class (photon trajectories)
├── AccretionDisk class (accretion disk)
├── RenderSystem class (rendering system)
├── Render thread (separate thread)
├── Console menu
└── SDL2 main loop
```

## ⚠️ Known Issues and Solutions

### Issue: High CPU Load
**Solution**: The program is specifically optimized for maximum performance. 
High CPU load is expected behavior.

### Issue: Black Screen on Launch
**Solution**:
1. Check if SDL2.dll is next to EXE
2. Update GPU drivers
3. Run as administrator

### Issue: Low FPS
**Solution**:
1. Reduce black hole mass in settings
2. Disable accretion disk
3. Disable photon trajectories

## 🔮 Development Plans

- [ ] Textured event horizon
- [ ] Flight mode through accretion disk
- [ ] Screenshot and video capture
- [ ] VR mode support
- [ ] Reissner-Nordström metric implementation (charged black hole)

## 📝 License

This project is distributed for educational purposes. 
You may freely use, modify, and distribute the code with attribution.

## 👨‍💻 Author

Developed as a demonstration of Kerr black hole physical effects.
Optimized C++ version using SDL2.

## 📞 Support

If you encounter issues:
1. Check SDL2 settings
2. Ensure OpenGL 3.3+ support
3. Check file permissions

For questions and suggestions, create Issues in the project repository.

---

**⚠️ WARNING**: The simulation creates significant CPU load. 
It is recommended to close other resource-intensive applications before running.
