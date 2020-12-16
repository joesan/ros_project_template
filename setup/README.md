## Local development environment setup

### Pre-requisites:

You can either use CLion or VS Code or something else as your IDE, but I prefer to use VS Code as it is fucking free to use. The steps below is for you to download, install and setup VS Code and the necessary extensions.

1. Download & install VS Code from [here](https://code.visualstudio.com/download)

2. You then have to make VS Code ROS ready, for this do the following (set of plugins need to be installed):
   2.1 The  C/C++ plugin    - https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools
   2.2 CMake plugin         - https://marketplace.visualstudio.com/items?itemName=twxs.cmake
   2.3 ROS plugin           - https://marketplace.visualstudio.com/items?itemName=ms-iot.vscode-ros
   2.4 VS Code icons plugin - https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons

3. I usually prefer to have all my source code a header file that contains the copyright and license text. For this I'm using the [psionq file header](https://marketplace.visualstudio.com/items?itemName=psioniq.psi-header). Just install this extension. To configure this, you need to open the settings.json by navigating from File -> Preferences -> Settings and then follow as per the screenshot below.

[Edit Settings](https://github.com/joesan/ros-navigator/blob/master/setup/images/edit-settings-json-1.png)

As a starter you can use this template from [here](https://github.com/joesan/ros-navigator/blob/master/setup/settings.json)

TODO: Under documentation

