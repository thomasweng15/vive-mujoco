# vive-mujoco

## Setup

1. Install Mujoco 2.0 `mujoco200` into the `.mujoco/` directory and get a license key
2. Clone this repo into the `.mujoco/` directory
3. Get dependencies: put header, dll, and lib files into directories in `mujoco200/` as follows:
    * `bin/`
        * `glew32.dll`
        * `glew32.lib`
        * `openvr_api.dll`
        * `openvr_api.lib`
    * `include/`
        * `GL/glew.h` (make a new folder named GL)
        * `openvr.h`
4. Run makefile in `src/` to build `.exe` files in the `mujoco200/bin/` folder
    * Open VS2015 x64 Native Tools Command Prompt
    * Navigate to `src/` directory in repo
    * Run `nmake -f makefile`
5. Run the code after making by navigating to `mujoco200/bin/` and running `mjvive.exe ..\..\vive-mujoco\model\sawyer_rope.xml`

## Notes

* `mjvive.py` currently doesn't work
* `minivive.cpp` is `mjvive.cpp` without controllers