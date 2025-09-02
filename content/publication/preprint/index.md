---
title: "Predictive Trajectory-Tracking for Mobile Robot Control, with Particle-Swarm Optimization on MPSoC-FPGA"
authors:
- admin
date: "2025-09-30T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: The rise of real-time hardware architectures and their advanced algorithmic adoption has opened opportunities for extrapolation and experiments with Nonlinear Model Predictive Control (NMPC) in resource-constrained systems. The backbone solution to the NMPC in such a context is to guarantee the convergence in a convex Quadratic Program (QP). Recent research has shown that with appropriate parallelization at the computational and algorithmic level, the solver for NMPC's cost is achievable at sub 1 $\mu $ by using the stochastic global optimizer particle swarm optimisation (PSO). However, PSO is computationally expensive, especially for large-scale systems with long prediction horizons. The proposed method in this study demonstrates the stabilized system using reduced sampling frequency and long prediction horizons. For the experiment, we designed the optimizer-NMPC using the high-level synthesis (HLS) method to accelerate the computation cost. Additionally, this solution will be generalized to control autonomous systems with similar features. To this end, the hardware architecture that was chosen for this study is the UltraScale+ KR260, an evaluation FPGA-MPSoC for rapid prototyping and adoption with Robotic Operating systems (ROS)-based solution. The experimental results proved that the enhanced control accuracy could be achieved by embedding the optimizer for trajectory-prediction module would reduce the workload on the Application Processor Unit of the FPGA SoC.

# Summary. An optional shortened abstract.
summary: This work present the improvement in trajectory-prediction accuracy with the combination of Nonlinear Model Predictive Control (NMPC) model using Particle Swarm Optimization (PSO) as global optimiser.  

tags:
- NMPC
- PSO
- High level synthesis (HLS)
- Trajectory-prediction

featured: true

hugoblox:
  ids:
    arxiv: 1512.04133v1

links:
- type: preprint
  provider: arxiv
  id: 1512.04133v1
- type: code
  url: https://github.com/MinhNguy3n/nmpc_hls
- type: slides
  url: https://www.slideshare.net/
# - type: dataset
#   url: "#"
# - type: poster
#   url: "#"
# - type: source
#   url: "#"
# - type: video
#   url: https://youtube.com
- type: custom
  label: Custom Link
  url: http://example.org

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
#   focal_point: ""
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

This work is driven by the results in Sergio's [paper](https://ieeexplore.ieee.org/document/10265730) on NMPC with PSO.

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}
<!-- 
Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
