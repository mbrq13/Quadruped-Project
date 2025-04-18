# Quadruped_Project_Scandia
## Quadruped Robot

## Índice

1. [Descripcion de paquetes](./doc/packages_doc.md)
2. [Instalacion ROS2](./doc/install_ros.md)
3. [Quadruped descripion](quadruped_description/README.md)
4. [Quadruped gazebo](quadruped_gazebo/README.md)
5. [Test package](test_package/README.md)
6. [Robots sim](robots_sim/README.md)

## Configuración

1. ### Creación de espacio de trabajo
    ```bash
    cd ~
    mkdir -p quadruped_robot_ws/src
    ```
2. ### Descarga de repositorio
    ```bash
    cd quadruped_robot_ws/src
    git clone https://github.com/sergio100899/Quadruped_Project_Scandia.git 
    ```
3. ### Descargar e instalar dependencias
    ```bash
    cd ~/quadruped_robot_ws
    rosdep init
    rosdep update --rosdistro $ROS_DISTRO
    rosdep install -i --from-path src --rosdistro $ROS_DISTRO -y
    ```
4. ### Compilación de espacio de trabajo

    ```bash
    cd ~/quadruped_robot_ws
    source /opt/ros/humble/setup.bash 
    colcon build --symlink-install
    source install/setup.bash
    ```
