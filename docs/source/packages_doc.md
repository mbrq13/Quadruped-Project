## Descripcion de paquetes


1. ### Quadruped Description: 
    Este paquete de ROS almacena los archivos de modelado del robot en formato URDF y XACRO, así como los archivos .stl y .obj del robot. También contiene archivos de lanzamiento (launch) para visualizar el robot en RViz. [video](https://www.youtube.com/watch?v=CwdbsvcpOHM/"video")

2. ### Quadruped Bringup: 
    Este paquete de ROS incluye los controladores (drivers) para el hardware real, como cámaras y LiDAR. También contiene archivos de lanzamiento que permiten iniciar el robot tanto en simulación como en su versión física, integrando todas sus características en un entorno ROS.

3. ### Quadruped Control: 
    Este paquete de ROS gestiona los controladores de alto nivel (high-level control), que permiten controlar el movimiento del robot (como marcha y giro), así como hacerlo permanecer de pie. Además, incluye archivos de configuración y lanzamiento de los controladores.

4. ### Quadruped Firmware:
    Este paquete de microROS contiene todo el código que se cargará en el controlador, junto con algunos scripts para arrancar el controlador desde una Raspberry Pi o Jetson Nano.[repositorio](https://github.com/husarion/rosbot_xl_ros/tree/master/rosbot_xl_utils/rosbot_xl_utils)

5. ### Quadruped Gazebo: 
    Este paquete de ROS contiene los plugins necesarios para dotar la simulación en Gazebo de mayores capacidades, además de incluir archivos con las propiedades físicas necesarias para la simulación.
6. ### Quadruped Hardware interface: 
    Este paquete de ROS sirve como enlace entre microROS y ROS, ya que los tópicos expuestos por microROS deben ser lo más livianos posible. Esta capa de abstracción entre microROS y ROS hace que el sistema sea más modular.

7. ### Quadruped Interfaces: 
    En este paquete de ROS se definen las interfaces personalizadas que permiten la comunicación entre los nodos en ROS1. Aquí se encuentran los equivalentes a los mensajes y servicios.
8. ### Quadruped Nav: 
    1. #### Quadruped Slam:
        Paquete que contiene los algoritmos de SLAM (Simultaneous Localization and Mapping), los mapas generados y los archivos de configuración. Permite navegar y generar mapas del entorno.
    2. #### Quadruped Localization:
        Este paquete contiene los algoritmos de localización (AMCL) y sus archivos de configuración, permitiendo que el robot se localice en su entorno.
    3. #### Quadruped Path planner:
        Paquete que contiene los algoritmos para la generación y seguimiento de trayectorias.
9. ### Quadruped Vision
    Este paquete agrupa todas las funcionalidades relacionadas con la visión, como la detección de obstáculos y el reconocimiento del entorno, utilizando herramientas como TensorFlow y YOLO.

9. ### Test package
    Este paquete agrupa todos los códigos para su testeo.

10. ### Robots sim
    Este paquete agrupa otras simulaciones de robots para su inspección y prueba.