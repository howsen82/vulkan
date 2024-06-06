### Vulkan Installation

To get started, follow these steps:

1. Download and Install [Vulkan SDK](https://vulkan.lunarg.com/sdk/home).
   
   *Windows*

   ```
   https://sdk.lunarg.com/sdk/download/1.3.283.0/windows/VulkanSDK-1.3.283.0-Installer.exe
   ```

   *Ubuntu*

   ```
   https://sdk.lunarg.com/sdk/download/1.3.283.0/linux/vulkansdk-linux-x86_64-1.3.283.0.tar.xz

   sudo apt update
   sudo apt install vulkan-sdk
   ```

2. Install Python 3.12
   
   *Windows*
   
   ```
   https://www.python.org/ftp/python/3.12.3/python-3.12.3-amd64.exe
   ```

   *Ubuntu*

   ```
   sudo apt update && sudo apt upgrade -y
   sudo apt install python3 -y
   ```
   
   *3rd Party*

   ```
   sudo add-apt-repository ppa:deadsnakes/ppa
   sudo apt install python3.12.3
   ```

   *Installing Python from Source Code*

   ```
   sudo apt install wget build-essential libreadline-dev libncurses5-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libdb5.3-dev libc6-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev zlib1g-dev -y
   wget https://www.python.org/ftp/python/3.12.3/Python-3.12.3.tgz
   tar -xvf Python-3.12.3.tgz
   cd Python-3.12.3
   ./configure --enable-optimizations
   make -j4
   sudo make install
   python3.12 --version

   # Uninstall
   sudo apt remove --autoremove python3.13
   sudo add-apt-repository --remove ppa:deadsnakes/ppa
   sudo make uninstall
   ```

   ```
   # Pip for python3
   sudo apt install python3-pip -y
   pip3 --version

   # Virtual Environment
   sudo apt install virtualenv -y
   virtualenv myenv
   source myenv/bin/activate
   ```

3. Clone the Repository
   
   *Windows*

   ```
   https://github.com/git-for-windows/git/releases/download/v2.45.2.windows.1/Git-2.45.2-64-bit.exe
   git clone https://github.com/PacktPublishing/The-Modern-Vulkan-Cookbook
   ```

   Debian/Ubuntu

   ```
   sudo apt install git -y
   https://github.com/PacktPublishing/The-Modern-Vulkan-Cookbook
   ```

4. Open the Project in Visual Studio 2022
   
5. Build the Project: Within Visual Studio, you can choose to build the project for debugging or release. For learning purposes and when making changes to the code, it’s recommended to use the **Debug** build configuration. This allows you to step through the code and understand its execution flow. For simply running the executables, you can use the **Release** build configuration.