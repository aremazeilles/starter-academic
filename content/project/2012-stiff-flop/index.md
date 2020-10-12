---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Stiff-flop"
summary: "(2012-2015)"
authors: []
tags: [robotics, surgery, control]
categories: []
date: 2012-06-21T22:54:06+02:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

This activity was funded by the European project STIFF-FLOP.

# Summary

This project was motivated by the current limitations of modern laparoscopic and robot-assisted surgical systems that are due to restricted access through Trocar ports, lack of haptic feedback, and difficulties with rigid robot tools operating inside a confined space filled with organs.

Taking inspiration from biological manipulators, like the octopus arm, a soft robotic arm was designed for enabling access, through bending, to areas non directly accessible with standard rigid tools.

In the context of the project, we developed:

- a sensorised benchmarking platform for analyzing the interaction forces in between the STIFF-FLOP arm and objects with variable stiffness.
- a generic position-based controller, able to deduce the appropriate configuration of the arm modules to reach a desired tip pose. The modular inverse kinematics model enables considering different features for characterizing the modules configuration (chamber length, constant curvature, position, pressure)
- an extension of the inverse kinematics to include in the process the estimation of the appropriate pose of the standard robotic arm holding the STIFF-FLOP flexible structure, while maintaining the single point insertion constraint.
- an extension of the inverse kinematics, through secondary tasks, for reducing the extension of the modules, or limiting the contacts detected with the external world.

# Related videos

{{< vimeo 289568317 >}}
Realized in March 2014 under simulation, using ROS environment

These simulations are presenting some position-based system control.
The configuration of the modules are defined to reach a desired tip pose (position and orientation).
To do so, an inverse kinematics framework is used. In the first video, the configuration of each flexible modules is defined through the position of the module tip expressed in its base.
From the obtained system configuration, the chamber lengths of each module is deduced under the constant curvature assumption.

{{< vimeo 289568176 >}}
Realized in December 2015, under simulation, using ROS environment.

In the second experiment, the constant curvature assumption is not made anymore.
Each module dynamics is expressed through beam theory.
Nevertheless the general inverse kinematics framework remains the same.
This video also include the estimation of the STIFF-FLOP arm holders pose (presented trough the gray tube).
This holder must take into account the single point insertion constraint (visualized with the red disc).
This constraint is modeled and embedded within the global inverse kinematics using an adaptation of the spherical coordinates.

Work in collaboration with Fabrice Morin, Asier Fernandez, Julius Klein and Alfonso Dominguez.
