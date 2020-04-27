---
title: MPC of Variable-speed ACs for Demand Response in Smart Grids
summary: To directly control the operating frequency of ACs in response to high-granularity electricity price signals, i.e., 5-minute real-time electricity prices,in smart grids using MPC method.
tags:

- Data-driven Modelling 
- Demand Response
- Energy flexibility 
- Air conditioner
- Building Energy System
- Kalman Filter
- MPC 
- Optimisation
- Real-time pricing

date: "2019-03-11"

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

{{< figure src="2.jpg" title="Fig. Schematic diagram of MPC for building energy systems." lightbox="true" >}}

---

**Demo Video: How MPC works? **

{{< video src="MPC_video.mp4" controls="yes" >}}

Receding horizon optimization: Optimization→Decision→Optimization→Decision …

---

**About**

<font face="Roboto" color="black" size="4">In the context of smart grids, residential air conditioners, as the major contributors to home electricity bills and loads on electrical grids, need to be not only energy-efficient, but also grid-responsive to relieve power supply-demand imbalance. Existing demand response control strategies for residential air conditioners focus on single-speed type and mainly adopt temperature set point reset to respond to hourly day-ahead electricity prices. This study represents the first attempt to directly control the operating frequency of inverter air conditioners in response to high-granularity electricity price signals, i.e., 5-minute real-time electricity prices, using model predictive control method. 

A simplified room thermal model in the stochastic state-space representation and performance maps of an inverter air conditioner are developed and integrated for predicting the coupled thermal response of an air-conditioned room. A demand response-enabled model predictive controller is designed based on the coupled model to optimally control the operating frequency of the inverter air conditioner while taking account of all the influential variables including weather conditions, occupancy, and 5-min real-time electricity prices. A Kalman filter is adopted to estimate the unmeasurable variables and remove the noises in measurements. A TRNSYS-MATLAB co-simulation testbed is developed to test the thermal and energy performances of the model predictive controller. 

{{< figure src="1.jpg" title="Fig. Flow chart of online model predictive control for variable-speed ACs." lightbox="true" >}}

Results show that compared to the PID controller, the demand response-enabled model predictive controller can implement automatic and optimal precooling to improve occupant’s thermal comfort at the beginning of occupancy. Moreover, it can also reduce average power consumption during peak demand periods by 17.31% to 38.86% compared with the PID controller and reduce all-day electricity costs by 0.42% to 22.16%. The frequency-based model predictive control method enables residential inverter air conditioners to be more grid-friendly and cost-efficient.</font>

---

**Related Publication**

[Maomao Hu, Fu Xiao, John Bagterp Jørgensen, Shengwei Wang (2019). Frequency control of air conditioners in response to real-time dynamic electricity prices in smart grids. Applied Energy.]({{< ref "/publication/journal_paper/rn-939/index.md" >}})

[Maomao Hu, Fu Xiao (2018). Model Predictive Control of Inverter Air Conditioners Responding to Real-Time Electricity Prices in Smart Grids. 5th International High Performance Buildings Conference.]({{< ref "/publication/conference_paper/rn-938/index.md" >}})

---

