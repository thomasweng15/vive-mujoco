# vive-mujoco

## Setup

1. Install Mujoco `mjpro150` into the `.mujoco/` directory and get a license key
2. Clone this repo into the `.mujoco/` directory
3. Get dependencies: put header, dll, and lib files into directories in `mjpro150/`
4. Run makefile in `src/` to get the exe files in the `mjpro150/bin/` folder
    * Open VS2015 x64 Native Tools Command Prompt
    * Navigate to `src/` directory in repo
    * Run `nmake -f makefile`
5. Run the code after making by navigating to the `bin/` folder in `mjpro150/` and running `mjvive.exe ..\..\vive-mujoco\model\humanoid100.xml`

## Notes

* `mjvive.py` currently doesn't work
* `minivive.cpp` is `mjvive.cpp` without controllers