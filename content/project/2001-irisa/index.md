---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Visual servoing"
summary: "Work conducted at IRISA (2001-2006)"
authors: []
tags: []
categories: []
date: 2006-06-22T00:50:00+02:00

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
<h2> Research activity at IRISA (2001-2006)  </h2>

  <p> My research performed at <a target="_blank"
    href="http://www.irisa.fr/">IRISA</a> was involved within French
    national projects <a target="_blank"
    href="http://jazz.ensil.unilim.fr/bodega/">Predit Mobivip</a> and <a
    target="_blank" href="http://www-sop.inria.fr/mobivip/">Robea
  Bodega</a>.
  During these years in Bretagne, I was member of the research
  projects <a target="_blank" href="http://www.irisa.fr/lagadic/">
  Lagadic</a> and <a target="_blank" href="http://www.irisa.fr/texmex">
  Texmex</a>.</p>

  <h3> Robotic navigation </h3>
  <p> This work concerns a topological approach of vision-based navigation.
    Within this framework, the navigation space is described by an image data-base acquired off-line.
    The localization of the robotic system is performed by using image retrieval methods.
    Indeed, as long as the current position of the robotic system is defined by the image acquired by the en-boarded camera, the localization is nothing but the search of the views from the database that are the most similar in term of content.
    The database is organized in a connectivity graph which gives a nice solution for defining a path between two images respectively describing the initial and desired positions, by performing a shortest path search.
    Original visual servoing methods are then proposed to control in-line the robot motions, by comparing the current view and the image path. </p>

  {{< vimeo 376657546 >}}

  <p> This work has been integrated onto the robotic car Cycab that belongs to IRISA.
    These experiments in real environments have shown the efficiency of the approach, and also its robustness towards illumination changes, local signal disturbance, visual sensors.
    It did enabled also to shed the light on critical parts that should be investigated for improving the current version.
    <br>Work in collaboration with <a target="_blank"
    href="http://www.irisa.fr/lagadic/team/Sinisa.Segvic-en.html">Sinisa
  Segvic</a>, <a target="_blank"
  href="http://www.irisa.fr/lagadic/team/Albert.Diosi-en.html">Albert
Diosi</a>, <a target="_blank"
href="http://www.irisa.fr/texmex/people/gros/index_en.htm">Patrick
Gros</a> and <a target="_blank"
href="http://www.irisa.fr/lagadic/team/Francois.Chaumette-en.html">François
Chaumette</a>.</p>

<h3>Landmarks management and tracking during navigation</h3>
<p>Developing an autonomous vision-based navigation system imposes to
  deal with the recognition of some visual information than can be
  extracted from the views acquired by the camera.
  These landmarks have
  also to be put in relation with the ones detected onto the image
  path.
  The use of a differential tracker manages to estimate within
  each acquired view the position of landmarks (Harris points) that were
  visible in the previous image.
  We are currently working on the
  improvement of such trackers to suit well to mobile vehicle
  characteristics (some results <a target="_blank"
  href="http://www.irisa.fr/lagadic/demo/demo-point-tracking-segvic/demo-segvic.html">here</a>).</p>

  <p> During the navigation, the environment observed by the camera
    continuously change.
    Therefor, the problem of automatic update of
    visual landmarks must be considered.
    A method based on image transfer
    is developed for detecting the apparition of landmarks from the image
    path within the camera field of view.
    Within this framework, no 3D
    model is needed, since a local reconstruction is sufficient.
    This
    approach has been tested and validated during the real experiments
    performed with the Cycab. <br> Work in collaboration with <a
    target="_blank"
    href="http://www.irisa.fr/lagadic/team/Francois.Chaumette-en.html">François
  Chaumette </a> and <a target="_blank"
  href="http://www.irisa.fr/lagadic/team/Sinisa.Segvic-en.html">Sinisa
Segvic </a>.</p>

<h3> Related videos</h3>

{{< vimeo 289569522 >}}
{{< vimeo 289570359 >}}

<p> These videos illustrate navigation in 3D environment. These simulations enable to study the control behavior, skipping the tracking step. </p>

<p> On the first video, 5 degrees of freedom of the camera are controlled (rotations around the optical axis are not considered). On the second video, the camera moves on a plan, like a holonomous mobile moving in a corridor.</p>

{{< vimeo 289569242 >}}

<p> This video illustrates a vision-based navigation task.
The environment is here planar, and the camera is mounted onto the effector of a Cartesian arm. </p>
<p> An image data-base is used to describe the environment that should observe the camera during its navigation.
 The features matched between each consecutive couple of images are used to control the motion of the robotic system (on the video the indexes displayed correspond to the couple of images from the path where these features were initially
extracted and matched). </p>
<p> All the displayed crosses are tracked in real-time with an exhaustive correlation.
The green features are the one used to control the robotic arm.
A planar homography is used to estimate the position of new features entering the camera field of view. </p>
<p>At the end of the sequence, a classical image-based visual servoing is performed.
The blue crosses correspond to the final
desired point positions. </p>

{{< vimeo 289569179 >}}
{{< vimeo 289569107 >}}

 <p> These two videos illustrate my first work on the extension of classical visual servoing for performing large displacements. </p>

<p>   An image path (obtained by image retrieval and shortest path finding) describes the visual environment that should observe the camera during the navigation. At each instant, an image-based visual servoing is used to make the visual features converge toward their positions observed in the next image of the path. </p>

<p> Here, we use the fact that the scene is planar. An homography is estimated between the current a nd desired positions of the features. This homography is used to project onto the current image plane the features matched with next image of the path. When enough are visible, the current servoing is stopped, and the next one is started. Thus, the camera does not converge toward each image of the path. </p>

<p>   In the second video, a path planning is performed at each beginning of visual servoing. It enables to estimate for each instant the best image position of the features. By using these positions as the desired features, one gets a constant velocity visual servoing.</p>
<p>   The red points are the points tracked. Blue points are the desired positions of these points. Green points are the desired positions of points not yet visible. In the second video, the blue points are the desired positions estimated by path planning. </p>

<p> Realized on the robotic arm Afma6 from the Lagadic project, IRISA. </p>
<p> With: <a target="_blank"  href="http://www.irisa.fr/texmex/people/gros/index_eng.htm">Patrick Gros </a>, <a target="_blank" href="http://www.irisa.fr/lagadic/team/Francois.Chaumette-eng.html">François Chaumette </a> and <a target="_blank"  href="http://wwwlasmea.univ-bpclermont.fr/spip.php?article222">Youcef Mezouar </a> </p>

<h3> Qualitative visual servoing </h3>

<p>An approach derived from classical visual servoing, called
  qualitative visual servoing, is proposed to control the motion of a
  robotic system.
  The main property of this control law is that it does
  not require visual features to converge exactly towards a desired
  value, but rather towards a confident interval.
  We are currently
  studying the theoretical properties of this original scheme, and
  through this work, considering the behavior of control laws that use a
weigthing matrix to activate or inactivate visual features. </p>

As an introduction, the qualitative visual servoing has been presented and firstly used for controlling the visibility of points during a positioning task.
Further works engaged are investigating the other applications that could benefit from this concept.

{{< vimeo 289567583 >}}
{{< vimeo 289566583 >}}

<p> This video presents an application of the qualitative servoing. Qualitative features are used to define a visibility constraint during a positioning task by visual servoing. </p>

<p> The qualitative visual servoing relies on the use of a weighting matrix for activating or inactivating features within the control law. The weight is obtained with a function that realizes a continuous heavyside transition between 0 (total inactivation) and 1 (full activation). </p>

<p> In these two experiments, a qualitative feature is associated to each point tracked and used within the control law. This qualitative features corresponds to the distance between the considered point and a confident area defined within the image plane. This feature is activated only when the point is close to the confident are borders. The additive constraint makes the camera modify its motion to keep the point inside its field of view. </p>

<p> Both videos present the trajectory of the camera with and without the qualitative features. If no visibility constraint is used, some features gets out the camera field of view in the first video. In the second video, the positioning tasks fails (classical problem of large rotation around the optical axis). By considering the visibility constraint with qualitative features, no point is lost in the first experiment, and the second one succeeds.</p>


Work in collaboration with <a target="_blank"
  href="http://www.irisa.fr/lagadic/team/Nicolas.Mansard-en.html">Nicolas
Mansard</a> and <a target="_blank"
href="http://www.irisa.fr/lagadic/team/Francois.Chaumette-en.html">François
Chaumette</a>.

