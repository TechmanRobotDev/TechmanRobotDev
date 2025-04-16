# Overview
Welcome! This GitHub page is dedicated to helping developers explore and understand the capabilities of secondary development with TM AI cobots. At Techman Robot, we believe that developers are the driving force behind innovation and creativity in robotics. Your vision, creativity, and expertise are what push the boundaries of what is possible with TM AI cobots. We are committed to providing you with powerful and flexible tools and a range of features tailored to bring your ideas to life. Here, we introduce 3 different fields of development you can explore on our robotics platform:
- Programming on Robot
- Remote Control
- Custom Plugins

# Programming on Robot
When developing your application locally using our software, TMflow, you have the flexibility to choose between two project types: Flow Project and Script Project. The Flow Project allows you to create block diagrams using a variety of function nodes, enabling you to build your application visually. With its intuitive “Drag, Drop, Develop” approach, this method is particularly user-friendly, making it an ideal choice for beginners in robotics. For more detailed information on programming a Flow Project, please refer to ___Software Manual – TMflow.___

On the other hand, the Script Project is designed for creating project using TMscript. TMscript is a powerful programming language developed by Techman Robot. TMscript offers advanced functionality that empowers experience engineers to delve into complex logic programming, providing the flexibility to edit, manage, and optimize robot tasks through code compilation. Additionally, TMscript can be seamlessly integrated into Flow Projects through the use of Script Nodes and Listen Nodes, enabling a hybrid approach that combines visual and code-based programming. For a deeper understanding of TMscript and its capabilities, please refer to the manual, ___Programming Language – TMscript.___

# Remote Control
For developers looking to develop their projects on broader systems and to control the robot remotely, our platform offers the following features and tools:
### Listen Server for motion control
Listen Server is a socket-based server designed to receive TMscript from external system, enabling remote control of robot motions. You can activate the Listen Server by running Listen Node within a flow Project, or by executing the TMscript function _ScriptLsten()_ within a Script Node or Script Project. For comprehensive guidance on utilizing the Listen Server and TMscript, please refer to the detailed instructions provided in the manual, _**Programming Language – TMscript**_.

### Servers for data acquisition & configuration
For data acquisition and system configuration, TMflow integrates multiple servers with different protocols, including Modbus, Ethernet, and optional support for Profinet and Ethernet-IP. Through these versatile servers, users can seamlessly gather system data, configure parameters, ensuring a flexible and robust integration with various industrial environments.
<table>
  <tr>
    <td>Check Robot Status</td>
    <td>Check Current TCP</td>
    <td>Check Joint Data</td>
  </tr>
  <tr>
    <td>Read or Write IOs</td>
    <td>Check or Assign Project</td>
    <td>Mimic Robot Stick</td>
  </tr>
  <tr>
    <td>Check Safety IOs</td>
    <td>Change Project Speed</td>
    <td>Check Configurations</td>
  </tr>
  <tr>
    <td>Check Robot Position</td>
    <td>Check Project Runtime</td>
    <td>Etc.</td>
  </tr>
</table>

### TM ROS Repository
For ROS developers, Techman Robot offers a suite of repositories tailored to various ROS versions, providing the tools necessary to seamlessly integrate TM AI cobots into your ROS-based projects. These repositories include:
- TM ROS Driver
- 3D Models of Various Robot Model Types
- Launch Files for TM AI cobot integration with Gazebo and Moveit

The TM ROS Driver enables developers to control robot motion via ROS Services and access robot data through ROS Topics. This comprehensive support allows for efficient simulation, planning, and execution of robotic tasks within the ROS ecosystem. For more detail, please visit: https://github.com/TechmanRobotInc

### EIH Camera API
For developers who have their own vision algorithms and wish to leverage the Eye-In-Hand (EIH) camera on the TM AI cobot, the EIH Camera API provides the tools you need. This API allows you to access raw image data directly from the camera, as well as retrieve and modify camera configurations, such as:
<table>
  <tr>
    <td>Camera Matrix</td>
    <td>Distortion Coefficients</td>
    <td>Hand Eye Array</td>
  </tr>
  <tr>
    <td>White Balance</td>
    <td>Pixel Format</td>
    <td>Image Size</td>
  </tr>
  <tr>
    <td>Focus Value</td>
    <td>Shuttle Time</td>
    <td>Etc.</td>
  </tr>
</table>

For more detail, please download the package **EIH Camera API proto** from Techman Download Center (Support software/EIH Camera API). This package includes:
- 2 proto files required for gRPC communication to the API
- Function manual

## Custom Plugins
At Techman Robot, we believe that by providing the right tools and platform, third-party developers can transform their fresh perspectives and ideas into groundbreaking solutions. These contributions not only enhance the capabilities of TMflow but also significantly enrich the overall user experience. Custom Plugins can particularly valuable in several key scenarios, including:
- At Techman Robot, we believe that by providing the right tools and platform, third-party developers can transform their fresh perspectives and ideas into groundbreaking solutions. These contributions not only enhance the capabilities of TMflow but also significantly enrich the overall user experience. Custom Plugins can particularly valuable in several key scenarios, including:
- Device Manipulation: Assisting engineers in seamlessly integrating and controlling third-party device on the robot, such as grippers, actuators, and other peripherals.
- Application Setup Wizards: Streamlining the process of building complex applications, like welding or palletizing, by guiding engineers through intuitive, step-by-step configurations.
- Custom Dashboards: Creating tailored displays that provide insights and monitoring specific to your application, enhancing operational efficiency and oversight.

Within TMflow, developers have two options for building custom plugins: TM Components and TMcraft plugins. Each offers unique opportunities to extend the software’s functionality, enabling developers to create tailored, innovative features that elevate the performance and versatility of our robotic systems.

### TM Components
TM Component is a kind of customized node that can be used on a flow project, just like other nodes. Using TM Component Editor, developers can design a sequence of nodes, variables, configurations, and package them into a TM Component. While its user interface customization is somewhat limited, the TM Component is straightforward to build and to test, making it an efficient solution for those looking to extend the functionality of TMflow with minimal complexity. For more details, please refer to _**Software Manual – TMflow, TM Component Editor**_.

### TMcraft Plugins
TMcraft is a robust architecture that enables developers to create plugins or background program directly embedded onto TMflow. Build on C# and WPF, TMcraft offers extensive customization options for the user interface, allowing developers to craft highly tailored solutions. Additionally, it can leverages the vast resources and libraries available within the developer community. With TMcraft API, these plugins can seamlessly interact with TMflow, enhancing the platform’s functionality and providing a more integrated user experience. For more detail, please visit: https://github.com/TechmanRobotDev/TMcraftDevelopmentKit

<!---
TechmanRobotDev/TechmanRobotDev is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
