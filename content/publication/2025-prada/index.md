---
title: "Flexible Constraint-Based Controller Framework for Ros_Control"
date: 2025-08-11
publishDate: 2025-08-11T21:56:15.919220Z
authors: ["M. Prada", "A. Fernandez", "A. Remazeilles", "J. McIntyre", ]
publication_types: ["2"]
abstract: "Generating robot behaviors in dynamic real-world situations generally requires the programming of multiple, often redundant degrees of freedom to meet multiple goals governing the desired motions. In this work, we propose a constraint-based controller specification methodology. A novel declarative language is used to combine semantically specialized building blocks into composite controllers. This description is automatically transformed at runtime into an executable form, which can automatically leverage multiple threads to parallelize computations whenever possible. Enabling runtime definition of controller topologies out of declarative descriptions not only reduces the work required to develop such controllers, but it also allows one to dynamically synthesize new controllers based on higher-level task planners or by user interaction through Graphical User Interfaces (GUIs). Our solution adds new functionality to the Robot Operating System (ROS)/ros_control ecosystem, where robot behaviors are typically achieved by deploying single-objective, off-the-shelf controllers for tasks like following joint trajectories, executing interpolated point-to-point motions in Cartesian space, or for basic compliant behaviors. Our proposed constraint-based framework enhances ros_control by providing the means to easily construct composite controllers from existing primary elements using our design language. Building on top of the ros_control infrastructure facilitates the usage of our controller with a wide range of supported robots and enables quick integration with the existing ROS ecosystem."
featured: false
publication: "*Robotics*"
tags: ["constraint-based control", "optimization", "ROS", "ros_control"]
doi: "10.3390/robotics14080109"
projects: ["2021-tracebot"]
---
