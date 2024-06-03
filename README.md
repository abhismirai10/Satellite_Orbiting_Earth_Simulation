# Satellite Orbiting Earth Simulation

This repository contains a Blender simulation of a satellite orbiting Earth, designed to generate datasets for algorithms such as Gaussian Splitting and Neural Radiance Fields (NeRF). The simulation is created using Blender 4.0 or higher.

## Contents

- [Description](#description)
- [Preview Video](https://youtu.be/rEmmlN9yqSI)
- [Installation](#installation)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

## Description

The simulation showcases a satellite orbiting Earth, capturing data for use in various computational algorithms. This simulation can be utilized for research and development in fields related to computer vision, machine learning, and 3D graphics.

### Scale and Measurements

The simulation uses a 1:10000 scale model. The key measurements are as follows:

- **Earth Diameter:** 12756 km → 127.56 m in simulation
- **Atmosphere Thickness:** 100 km → 1 cm in simulation
  - **Total Diameter with Atmosphere:** 12856 km → 128.56 m
- **Satellite Size:** 10 m → 0.001 m in simulation
- **Low Earth Orbit (LEO):** 500 km above Earth surface → 50 m in simulation

The satellite orbits approximately 50 m + (127.56 m / 2) ≈ 113.78 m from the Earth's center in the simulation.
![untitled](https://github.com/abhismirai10/Satellite_Orbiting_Earth_Simulation/assets/121724635/7eab0dbb-c426-4a92-a2b9-f11ae0912bff)


## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/yourusername/satellite-orbit-simulation.git
   cd satellite-orbit-simulation
   ```

2. **Install Blender 4.0 or higher:** Follow the [official Blender installation guide](https://www.blender.org/download/). set folder's name and hierarchy as described in [Folder Structure](#folder-structure) section.

3. **Open Blender and load the scene:**

   Open Blender, navigate to the `Scene` folder, and open `satellite_earth_model_for_3DGS.blend`.

4. **Generate Simulation:**

   - Adjust settings as needed (e.g., resolution, rendering details, animation settings) or click render->render animation to generate data with
     default settings.
   - Alternatively, run the script `orbit_around_satellite.py` to automate the process.


## Folder Structure

The repository is organized as follows:

```
Satellite_Orbiting_Earth_Simulation/
├── Scene/
│   ├── satellite_model.blend
│   ├── earth_model.blend
│   ├── satellite_earth_model.blend
│   ├── satellite_earth_model_for_3DGS.blend
│   └── Datasets/
│       └── "will have generated dataset"
├── Textures/
│   └── "Download and Paste earth texture from the given link"
├── Scripts/
│   └── orbit_around_satellite.py
```

- `Scene/`: Contains all scene-related files.
  - `satellite_model.blend`: Blender file for the satellite model.
  - `earth_model.blend`: Blender file for the Earth model.
  - `satellite_earth_model.blend`: Blender file for the combined satellite and Earth model.
  - `satellite_earth_model_for_3DGS.blend`: Blender file for the combined satellite and Earth model specifically for 3D Gaussian Splitting.
- `Textures/`: Folder containing texture files for the models.
  - Download and paste the Earth texture from the provided [link](https://www.dropbox.com/scl/fo/f2skfbz0rla3fsx6obozq/ALqcuBhd0nejWNdZuNJWIzk?rlkey=mhp62ord46wv7kt8afqhm20dq&e=1&dl=0). (first unzip the folder and rename it to "Textures" and paste)
- `Scripts/`: Folder for any Blender Python scripts used in the simulation.
  - `orbit_around_satellite.py`: Script to control the satellite's orbit around Earth.
- `Datasets/`: Folder to store generated datasets.
  - Will contain datasets generated from the simulation.

## Contributing

We welcome contributions to improve the simulation. If you have any suggestions or enhancements, please fork the repository, create a new branch, and submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request

## License

Be nice to each other. enjoy!

---
