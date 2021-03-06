# CHAMP Setup Assistant
This software auto generates a configuration package containing all the [files](https://github.com/chvmp/champ_setup_assistant/tree/master/templates) necessary to make CHAMP walk. 

![CHAMP Setup Assistant](https://raw.githubusercontent.com/chvmp/champ_setup_assistant/master/docs/images/setup.png)
## Installation

1. Clone and install all dependencies:

        sudo apt install -y python-rosdep
        cd <your_ws>/src
        git clone https://github.com/chvmp/champ_setup_assistant
        cd ..
        rosdep install --from-paths src --ignore-src -r -y

2.  Build your workspace:

        cd <your_ws>
        catkin_make
        source <your_ws/>/devel/setup.bash

## Quick Start

1. Run the setup assistant:

        roslaunch champ_setup_assistant setup_assistant.launch 

Configure your robot by loading a URDF or manually key in the configuration parameters. If you don't have any URDF now, you can download [ANYmal](https://github.com/chvmp/anymal_b_simple_description/tree/master/urdf) or [SpotMicro](https://github.com/chvmp/spotmicro_description/blob/master/urdf/spotmicroai.urdf) just to try the package.