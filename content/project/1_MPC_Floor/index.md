---
title: MPC of Floor Heating Systems in Denmark
summary: To develop model predictive control for floor heating systems to provide energy flexibiltiy. The proposed MPC can simultaneously consider all the influential variables including weather conditions, occupancy and dynamic electricity prices.
tags:
- Data-driven Modelling 
- Demand Response
- Energy flexibility 
- Floor heating
- Building Energy System
- Kalman Filter
- MPC 
- Optimisation
- Real-time pricing

date: "2019-02-14"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: by Maomao Hu
  focal_point: Smart

# links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#   slides: example

---

{{< figure src="RC_floor.jpg" title="Fig. Schematic of the grey-box RC model for floor heating systems" lightbox="true" >}}

{{< figure src="MPC_scheme.jpg" title="Fig. Flow chart of online model predictive control for floor heating systems." lightbox="true" >}}

**About**

<font face="Roboto" color="black" size="4"> Floor heating (FH) system is a widely-used thermally active building system, which can take advantage of building thermal mass to shift energy demands to off-peak hours. Its ability of effective  utilization of low-temperature energy resources also helps to increase energy efficiency and reduce greenhouse gas emissions. However, control of FH systems remains a challenge due to the large thermal inertia of the pipe-embedded concrete floor. In the context of smart grids, the control issue becomes more complicated because the dynamic electricity prices need to be taken into consideration to achieve economic benefits and encourage demand response participation. 

In this study, an advanced optimal control method, i.e., model predictive control (MPC), is developed for FH systems, which can simultaneously consider all the influential variables including weather conditions, occupancy and dynamic electricity prices. Considering the on-line computational efficiency, a control-oriented dynamic thermal model for a room integrated with FH system is developed and represented in a stochastic state-space form. An economic MPC controller, formulated as a mixed integer linear programming problem, is designed for FH systems. A TRNSYS-MATLAB co-simulation testbed is developed to test and compare different control methods under various operating conditions in terms of energy consumption, thermal comfort and operating costs. 

Test results show that, compared to the conventional on-off controller, the MPC controller is able to use building thermal mass to optimally shift energy consumption to low-price periods, improve thermal comfort at the beginning of occupancy, reduce energy demand during peak periods, and save electricity costs for residential end-users. The weather conditions and electricity prices have influences on the start-up time and duration of preheating, energy flexibility potential and electricity cost savings of FH systems. </font>

---

**Acknowledgement**

The presented work receives the support of the [CITIES project](http://smart-cities-centre.org/), the SCA project, and the [EnergyLab Nordhavn project](http://www.energylabnordhavn.com/) in Denmark. 

---

**Related Publication**

[Maomao Hu, Fu Xiao, John Bagterp Jørgensen, Rongling Li (2019). Price-responsive model predictive control of floor heating systems for demand response using building thermal mass. Applied Thermal Engineering.]({{< ref "/publication/journal_paper/rn-935/index.md" >}})

---

