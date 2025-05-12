# Software Setup

1. ## Creación de espacio de trabajo
    ```bash
    cd ~
    mkdir -p quadruped_robot_ws/src
    ```
2. ## Descarga de repositorio
    ```bash
    cd quadruped_robot_ws/src
    git clone https://github.com/sergio100899/Quadruped_Project_Scandia.git 
    ```
3. ## Descargar e instalar dependencias
    ```bash
    cd ~/quadruped_robot_ws
    rosdep init
    rosdep update --rosdistro $ROS_DISTRO
    rosdep install -i --from-path src --rosdistro $ROS_DISTRO -y
    ```
4. ## Compilación de espacio de trabajo

    ```bash
    cd ~/quadruped_robot_ws
    source /opt/ros/humble/setup.bash 
    colcon build --symlink-install
    source install/setup.bash
    ```
