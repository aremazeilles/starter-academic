---
title: "Minimum Cost Averaging for Multivariate Time Series Using Constrained Dynamic Time Warping: A Case Study in Robotics"
date: 2023-07-01
publishDate: 2023-07-04T21:56:15.919220Z
authors: ["I. Rasines", "A. Remazeilles", "M. Prada", "I. Cabanes"]
publication_types: ["2"]
abstract: "In this paper, an innovative algorithm for averaging a set of multivariate time series with different lengths based on Constrained Dynamic Time Warping (CDTW) is proposed. This approach relies on the CDTW to provide the non-linear alignment of the multivariate time series, and employs the proposed Minimum Cost Averaging (MCA) technique to identify the optimum matches and get equal-length time series. MCA-CDTW is a task-agnostic approach that after selecting a reference curve, transforms the rest of the demonstrations in the set to obtain new curves that are time-aligned with the reference. From these transformed curves, not only the mean but also the signal variability can be directly extracted. This technique provides smooth mean curves even when there are large deviations between the demonstrations in the set, and still the complexity of the proposed algorithm is significantly reduced compared to other averaging techniques from the literature. When learning techniques are used to teach a motion to a robotic system, obtaining smooth trajectories is important to achieve good robotic behaviors. The new algorithm MCA-CDTW is tested and compared on two different databases: a literature database where humans move a robotic arm with kinaesthetic teaching, and a set of recordings of a teleoperated robotic arm performing laboratory manipulation. On both datasets, it is demonstrated that the new approach is providing smooth average trajectories."
featured: false
publication: "*IEEE Access 2023*"
tags: ["Dynamic time warping", "jerk cost", "multivariate time series", "smoothness", "time series averaging"]
doi: "10.1109/ACCESS.2023.3300720"
url_pdf: "https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10198412"
projects: ["2021-tracebot"]
---
