# HT_urdf


## Installation

```bash
pip install -e .
```

## Usage example
``` python
import ht_urdf
ht_urdf_path = os.path.dirname(ht_urdf.__file__)
self.scene.robot.spawn.asset_path = f"{ht_urdf_path}/PiPlus_S_12L10A0G0H1W/PiPlus_S_12L10A0G0H1W.urdf"
```
## Project Structure

```
ht_urdf/
├── setup.py                                    # Installation configuration
├── README.md                                   # Project documentation
└── ht_urdf/                                    # Main package directory
    ├── __init__.py                             # Package initialization
    └── PiPlus_S_12L10A0G0H1W/                 # Robot model package
        ├── PiPlus_S_12L10A0G0H1W.urdf         # URDF robot description file
        ├── CMakeLists.txt                      # CMake build configuration
        ├── config/                             # Configuration files
        │   └── joint_names_PiPlus_S_12L10A0G0H1W.yaml  # Joint names configuration
        ├── meshes/                             # 3D mesh files (STL format)
        │   ├── base_link.STL
        │   ├── torso_link.STL
        │   ├── head_*.STL                      # Head links
        │   ├── l_*.STL                         # Left side links
        │   ├── r_*.STL                         # Right side links
        │   └── waist_yaw_link.STL
        ├── launch/                             # ROS launch files
        │   ├── display.launch                  # RViz visualization
        │   └── gazebo.launch                   # Gazebo simulation
        └── xml/                                # Additional XML files
```

## License

BSD-3-Clause
