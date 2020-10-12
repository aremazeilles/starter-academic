---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "SAM"
summary: "a robotic butler for injured people (2006-2008)"
authors: []
tags: []
categories: []
date: 2006-06-22T00:46:46+02:00

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
## Research activity within  CEA (2006-2007)

This research was performed within two projects:

- The European project ITEA ANSO gathers about 15 partners working together for designing technical solutions towards a domotic environment.
- AVISO is a French project, in collaboration with the association Approche (assistance to disable people).
  This partnership will allow the CEA to evaluate with real end-users their scientific productions within several medical centers.

### Towards Robotic Assistance for injured people

  <p> In few words, the CEA research concerns the design of a robotic arm
   able to grasp objects within a apartment-like environment.
   A stereoscopic rig fixed onto the gripper is used
   to control the arm.
   The end-user defines onto a display an object to grasp (by simply defining a box around it), and a visual servoing task is performed to go and fetch the defined object.
 </p>

### Contribution to the project

 <p> Within this context, my work was to :
   <ul>
    <li> develop a stereo tracking algorithm. The main originality is
    that no object model is needed. </li>
    <li> design a control module (based on visual servoing  principles) to command the arm. </li>
  </ul>
</p>

<p> The development of such elements enabled me to define several scientific libraries dealing with :
  <ul>
   <li> algebra </li>
   <li> image grabbing </li>
   <li> camera calibration </li>
   <li> visual servoing </li>
   <li> feature extraction (harris points) and tracking (differential correlation), template matching (exhaustive correlation) </li>
   <li> pose estimation </li>
 </ul>
</p>

<p> Naturally, these libraries are now easily usable by the rest of the laboratory </p>

### The autonomous mobile robotic platform SAM

Within the ANSO project, all these hardware and software elements are embedded into a mobile platform (developed by Neobotix), which enables the user to perform a grasping wherever in his apartment.
This original application has the following skills:

- IHM designed for non specialists end-users, minimizing the number of interactions,
- Client /server mode enabling to interact with the mobile system, through a DPWS stack onto a wifi network,
- Action scheduling and monitoring controlled by a generic scenario interpretor layer,
- Autonomous mobile robot navigation (developed by Neobotix),
- Automatic object grasping (after a simple definition by the user).

### Related videos

{{< youtube wm6cPrmXfxE >}}
Realized during technical evaluations, in January 2008,  Morvan hospital, Brest, France.
{{< vimeo 276530873 >}}
Realized during the ITEA ANSO evaluation, September 2007 the 13, at the CEA of Fontenay aux Roses.

 <p> This video presents the general behavior of the mobile robotic platform SAM developed by the <a target="_blank"
        href="http://www-list.cea.fr/index_gb.htm">CEA-LIST</a>, for improving the well-being of disabled people.
      </p>
      <p> The mobile platform enables to go and grasp every-day_life objects within a domestic environment.
        From a remote friendly man-machine interface, the user ask the robot to reach a topological room (like the kitchen).
        When the mobile platform is within this place, the user defines the object to bring back, and the robotic arm realizes the grasping task.
      </p>
      <p>
        This global application naturally gathers several high-level technologies. One of the originalities, from the user part, is that the grasping task is very easy to start, and also generic.
        Simple because only two image clicks are necessary to select the object (this defines a box in which is the object of interest). Generic because no a priori information, like a 3D model, is used onto the object to grasp.
        Any textured object can thus be considered without changing the program.
      </p>

The robotic arm is designed by [Exact Dynamics](http://www.exactdynamics.nl/).
The mobile platform, and its navigation software, is a product of <a target="_blank"href="http://www.neobotix.de/en/">Neobotix</a>.

<p> Work in collaboration with Christophe Leroux, Gerard Chalubert, Martine Guerrand, Aline Chansavang, Céline Teulière & Mathieu le Cam.</p>
