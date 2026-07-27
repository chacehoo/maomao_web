---
title: 
summary: xxxx
date: 2024-01-08
weight: 5

reading_time: true
share: true
profile: true
comments: false
---

<style>
html,
body {
  scroll-behavior: auto !important;
}

.research-page {
  display: flex;
  align-items: flex-start;
  gap: 44px;
  max-width: 1500px;
  margin: 0 auto;
  padding: 0 24px;
}

.research-sidebar {
  width: 250px;
  flex: 0 0 250px;
  position: sticky;
  top: 100px;
  z-index: 100;
  background: #ffffff;
  padding: 0;
  margin: 0;
  border: none;
  box-shadow: none;
}

.research-sidebar a {
  display: block;
  position: relative;
  width: 100%;
  padding: 14px 16px 14px 18px;
  margin: 0 0 8px 0;
  border-radius: 0;
  border: 1px solid #e5e5e5;
  border-left: 5px solid transparent;
  background: #ffffff;
  color: #EF7C00;
  text-decoration: none;
  font-size: 1.02rem;
  line-height: 1.35;
  font-weight: 500;
  transition: none;
}

.research-sidebar a:hover {
  background: #f7f9fc;
  color: #003D7C;
  border-left-color: #EF7C00;
}

.research-sidebar a.active {
  background: #f7f9fc;
  color: #003D7C;
  border-left-color: #EF7C00;
  font-weight: 700;
}

/* Sidebar dropdown */
.sidebar-group {
  width: 100%;
}

.sidebar-parent {
  display: flex !important;
  align-items: center;
  justify-content: space-between;
}

.sidebar-arrow {
  font-size: 0.85rem;
  color: inherit;
  transition: transform 0.2s ease;
}

.sidebar-group.open .sidebar-arrow {
  transform: rotate(180deg);
}

.sidebar-submenu {
  display: none;
  margin: -2px 0 10px 0;
  padding: 0 0 0 18px;
  border-left: 2px solid #f0f0f0;
}

.sidebar-group.open .sidebar-submenu {
  display: block;
}

.research-sidebar a.sidebar-subitem {
  width: calc(100% - 18px);
  padding: 8px 12px 8px 18px;
  margin: 0 0 6px 0;
  font-size: 0.9rem;
  font-weight: 400;
  color: #6b7280;
  border: none;
  border-left: 4px solid transparent;
  background: transparent;
}

.research-sidebar a.sidebar-subitem:hover {
  color: #003D7C;
  background: #f7f9fc;
  border-left-color: #EF7C00;
}

.research-sidebar a.sidebar-subitem.active {
  color: #003D7C;
  background: #f7f9fc;
  border-left-color: #EF7C00;
  font-weight: 600;
}

.research-main {
  flex: 1;
  min-width: 0;
}

/* Section title: h2 */
.research-section-title {
  text-align: center;
  font-weight: 800;
  font-size: clamp(1.9rem, 3.2vw, 2.6rem);
  margin-top: 1.5rem;
  margin-bottom: 2.3rem;
  color: #EF7C00;
  scroll-margin-top: 120px;
}

.research-section-title::after {
  content: "";
  display: block;
  width: 52px;
  height: 4px;
  background: #EF7C00;
  margin: 12px auto 0 auto;
  border-radius: 999px;
}

/* Thrust title: h3 */
.research-subtitle {
  display: block;
  text-align: center;
  font-weight: 650;
  line-height: 1.25;
  color: #333333;
  margin-top: 2.4rem;
  margin-bottom: 1.1rem;
  scroll-margin-top: 120px;
}

.research-subtitle .title-line,
.research-subtitle .subtitle-line {
  display: block;
}

.research-subtitle .title-line {
  font-size: clamp(1.45rem, 2.4vw, 2rem);
  font-weight: 800;
  line-height: 1.2;
  color: #003D7C;
}

.research-subtitle .subtitle-line {
  max-width: 850px;
  margin: 0.65rem auto 0;
  font-size: clamp(1rem, 1.45vw, 1.2rem);
  font-weight: 600;
  line-height: 1.45;
  color: #333333;
}

.research-subtitle .thrust-label {
  color: #003D7C;
  font-weight: 800;
}

.research-card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 24px;
  width: 80%;
  max-width: 1050px;
  margin: 24px auto 48px auto;
}

.research-card-grid.three-cards {
  grid-template-columns: 1fr;
  width: 80%;
  max-width: 1050px;
  gap: 24px;
}

.research-card {
  margin: 0;
  background: #ffffff;
  border-radius: 18px;
  box-shadow: 0 8px 28px rgba(0, 0, 0, 0.07);
  overflow: hidden;
  text-align: center;
}

.research-card-image-wrap {
  width: 100%;
  background: #ffffff;
}

.research-card-grid.three-cards .research-card-image-wrap {
  aspect-ratio: 16 / 9;
  overflow: hidden;
}

.research-card img {
  width: 100%;
  height: auto;
  display: block;
}

.research-card-grid.three-cards .research-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.research-card iframe {
  width: 100%;
  aspect-ratio: 16 / 9;
  border: 0;
  display: block;
}

.research-card figcaption {
  padding: 14px 18px 18px 18px;
  line-height: 1.45;
  font-size: 0.98rem;
  background: #ffffff;
  color: #5f6876;
  text-align: center;
}

.research-card figcaption.left-caption {
  text-align: left;
  line-height: 1.65;
  font-size: 1.02rem;
}

/* All card links in NUS yellow */
.research-card figcaption a {
  color: #EF7C00 !important;
  font-weight: 500;
  text-decoration: none !important;
  margin-left: 6px;
}

.research-card figcaption a:hover {
  color: #003D7C !important;
  text-decoration: underline !important;
}

.access-note {
  display: block;
  margin-top: 4px;
  font-size: 0.82rem;
  font-weight: 400;
  color: #7a8491;
}

.research-overview-logo {
  display: flex;
  justify-content: center;
  margin-bottom: 1.4rem;
}

.research-overview-logo img {
  width: 78%;
  max-width: 760px;
  height: auto;
}

.research-tagline {
  text-align: center;
  margin-bottom: 2rem;
}

.research-main p,
.research-main li {
  color: #333333;
  line-height: 1.7;
}

code {
  background: none !important;
  border: none !important;
  padding: 0;
  box-shadow: none !important;
}

@media (max-width: 992px) {
  .research-page {
    display: block;
    padding: 0 16px;
  }

  .research-sidebar {
    width: 100%;
    position: static;
    margin-bottom: 28px;
  }

  .research-sidebar a {
    font-size: 0.98rem;
    padding: 12px 14px;
    margin-bottom: 8px;
  }

  .sidebar-submenu {
    padding-left: 14px;
  }

  .research-sidebar a.sidebar-subitem {
    font-size: 0.9rem;
    padding: 8px 12px 8px 16px;
  }

  .research-section-title {
    font-size: clamp(1.6rem, 7vw, 2rem);
  }

  .research-subtitle .title-line {
    font-size: clamp(1.25rem, 5.5vw, 1.6rem);
  }

  .research-subtitle .subtitle-line {
    font-size: clamp(0.95rem, 4vw, 1.05rem);
  }

  .research-card-grid {
    width: 100%;
    max-width: 100%;
  }

  .research-card-grid.three-cards {
    grid-template-columns: 1fr;
    width: 100%;
    max-width: 100%;
  }

  .research-overview-logo img {
    width: 100%;
  }
}
</style>

<div class="research-page">

<aside class="research-sidebar">
  <a href="#overview" class="active">Research Overview</a>

  <div class="sidebar-group">
    <a href="#research-thrusts" class="sidebar-parent">
      <span>Research Thrusts</span>
      <span class="sidebar-arrow">▾</span>
    </a>
    <div class="sidebar-submenu">
      <a href="#free-systems" class="sidebar-subitem">FREE energy systems</a>
      <a href="#digitalization" class="sidebar-subitem">Digitalization</a>
      <a href="#control" class="sidebar-subitem">Control</a>
      <a href="#ai" class="sidebar-subitem">AI</a>
    </div>
  </div>

  <a href="#research-center">Research Center</a>
  <a href="#testbeds">Living Testbeds</a>
</aside>

<main class="research-main">

<h2 id="overview" class="research-section-title">Research Overview</h2>

<div class="research-overview-logo">
<img src="bior_logo_light_background.png" alt="BIOR LOGO">
</div>

<div class="research-tagline">
<div id="typed-strings">
<p><code style="color: #EF7C00; font-weight: bold;">Smart</code></p>
<p><code style="color: #EF7C00; font-weight: bold;">Low-carbon</code></p>
<p><code style="color: #EF7C00; font-weight: bold;">Energy-efficient</code></p>
<p><code style="color: #EF7C00; font-weight: bold;">Demand-flexible</code></p>
<p><code style="color: #EF7C00; font-weight: bold;">Climate-resilient</code></p>
<p><code style="color: #EF7C00; font-weight: bold;">Equitable</code></p>
</div>
<span class="font-bold" id="typed"></span>
<code style="color: #003D7C">Building, District, and Urban Energy Systems.</code>
</div>

<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
<script>
var typed = new Typed('#typed', {
  stringsElement: '#typed-strings',
  typeSpeed: 50,
  backSpeed: 30,
  startDelay: 100,
  backDelay: 2000,
  loop: true
});
</script>

<p>
Our BIOR lab aims at developing sustainable and scalable technologies and computational tools to make building, district, and urban energy systems smart, low-carbon, energy-efficient, energy-flexible, climate-resilient, and equitable using optimization, learning, and control.
</p>

<p>
Our interdisciplinary research is at the interface of Building Science, Computer Science, and Control Engineering.
</p>

<p>
We employ a multifaceted approach that encompasses data analytics & machine learning, physics-based modeling & simulation, optimization & model-based optimal controls, as well as experiments. These approaches have been deployed across a spectrum of scales, spanning from equipment- through building- and community- to city-scale.
</p>

<p>Specifically, our research interests include:</p>

<ul>
<li><strong>FREE energy systems</strong>: Flexible, Resilient, Efficient, and Equitable (FREE) multi-scale building-integrated energy systems with distributed energy resources (DERs)</li>
<li><strong>Digitalization</strong>: Multi-scale digital twins (DT) and energy management information system (EMIS)</li>
<li><strong>Control</strong>: Model-based and learning-based optimal control</li>
<li><strong>AI</strong>: AI for building and urban science and engineering (AI4BUSE)</li>
</ul>

<h2 id="research-thrusts" class="research-section-title">Research Thrusts</h2>

<h3 id="free-systems" class="research-subtitle">
  <span class="title-line">
    <span class="thrust-label">Thrust 1: FREE energy systems</span>
  </span>
  <span class="subtitle-line">
    Flexible, Resilient, Efficient, and Equitable (FREE) multi-scale building-integrated energy systems with distributed energy resources (DERs)
  </span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/thrust_1_0.jpg" alt="Complex Cyber-Physical District Energy System">
</div>
<figcaption>
<div style="font-weight: 500;">Complex cyber-physical district energy system</div>
<div style="margin-top: 6px;">
<a href="https://doi.org/10.1016/j.enbuild.2023.113339" target="_blank" rel="noopener">[Link]</a>
<a href="https://sesi.stanford.edu/energy-systems/central-energy-facility" target="_blank" rel="noopener">[Link]</a>
</div>
</figcaption>
</figure>

<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/thrust_1_1.jpg" alt="Coordination and Negotiation in a Cyber-Physical Multi-Entity Residential Microgrid">
</div>
<figcaption>
<div style="font-weight: 500;">Coordination and negotiation in a cyber-physical multi-entity residential microgrid</div>
<div style="margin-top: 6px;">
<a href="https://doi.org/10.1016/j.rser.2020.110248" target="_blank" rel="noopener">[Link]</a>
</div>
</figcaption>
</figure>
</div>

<h3 id="digitalization" class="research-subtitle">
  <span class="title-line">
    <span class="thrust-label">Thrust 2: Digitalization</span>
  </span>
  <span class="subtitle-line">
    Multi-scale digital twins (DT) and energy management information system (EMIS)
  </span>
</h3>

<div class="research-card-grid three-cards">

<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/Urban_DT.png" alt="Urban Digital Twin">
</div>
<figcaption>
Urban Microclimate-Informed Digital Twins
<a href="https://urbandt.org/" target="_blank" rel="noopener">[Visit]</a>
</figcaption>
</figure>

<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/Campus%20EMIS.png" alt="NUS campus Energy Management Information System">
</div>
<figcaption>
NUS Campus EMIS
<a href="http://10.245.67.108:3000/login" target="_blank" rel="noopener">[Visit]</a>
<span class="access-note">(login required; NUS intranet only)</span>
</figcaption>
</figure>

<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/Building_Room_DT.png" alt="Building Digital Twin">
</div>
<figcaption>
Building Digital Twins
<a href="https://www.buildingdt.org/" target="_blank" rel="noopener">[Visit]</a>
<span class="access-note">(login required)</span>
</figcaption>
</figure>

</div>

<h3 id="control" class="research-subtitle">
  <span class="title-line">
    <span class="thrust-label">Thrust 3: Control</span>
  </span>
  <span class="subtitle-line">
    Model-based and learning-based optimal control
  </span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/thrust_2.jpg" alt="Schematic diagram of MPC for building energy systems">
</div>
<figcaption>
Schematic diagram of MPC for building energy systems
<a href="https://maomaohu.net/project/0_mpc_ac/" target="_blank" rel="noopener">[Link]</a>
<a href="https://maomaohu.net/project/1_mpc_floor/" target="_blank" rel="noopener">[Link]</a>
</figcaption>
</figure>
</div>

<h3 id="ai" class="research-subtitle">
  <span class="title-line">
    <span class="thrust-label">Thrust 4: AI</span>
  </span>
  <span class="subtitle-line">
    AI for building and urban science and engineering (AI4BUSE)
  </span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/thrust_3_0.jpg" alt="Explainable Machine Learning using Large-Scale Smart Meter Data">
</div>
<figcaption>
Explainable machine learning using large-scale smart meter data
<a href="https://maomaohu.net/software/ifeel/" target="_blank" rel="noopener">[Link]</a>
<a href="https://doi.org/10.1016/j.scs.2021.103380" target="_blank" rel="noopener">[Link]</a>
<a href="https://doi.org/10.1016/j.enbuild.2023.112896" target="_blank" rel="noopener">[Link]</a>
</figcaption>
</figure>
</div>

<h2 id="research-center" class="research-section-title">Research Center</h2>

<h3 class="research-subtitle">
  <span class="title-line">Center for Digital Building Technology</span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/center_for_digital_building_tech.jpg" alt="Center for Digital Building Technology">
</div>

<div class="research-card-image-wrap">
<iframe
src="https://www.youtube.com/embed/gY_YT0Vc8EA?si=YctpIQsh5_LxP-xr"
title="Centre for Digital Building Technology"
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
referrerpolicy="strict-origin-when-cross-origin"
allowfullscreen>
</iframe>
</div>

<figcaption class="left-caption">
Dr. Hu has served as the deputy director of the
<a href="https://cde.nus.edu.sg/dbe/centre-for-digital-building-technology/" target="_blank" rel="noopener">Center for Digital Building Technology</a>
since 2025. The center's primary mission is to enhance quality and productivity by leveraging digital building technologies to transform how people design, deliver, and manage the built environment. These technologies include augmented reality (AR), virtual reality (VR), building information modeling (BIM), the Internet of Things (IoT), robotics and automation, video analytics, and digital twins, all supported by advanced equipment and devices.
</figcaption>
</figure>
</div>

<h2 id="testbeds" class="research-section-title">Living Testbeds</h2>

<h3 class="research-subtitle">
  <span class="title-line">SDE 4, a net-zero energy building</span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/PV_2.png" alt="SDE 4, a net-zero energy building">
</div>

<figcaption class="left-caption">
SDE4 is Singapore’s first new-build net-zero energy building, designed to exemplify human-centric and integrated sustainable development. Completed in 2019, the six-story structure incorporates passive design strategies, including a large overhanging roof and double facades on its east and west sides, to provide shading and minimize solar heat gain. Its hybrid cooling system enhances energy efficiency by maintaining comfortable indoor temperatures without excessive cooling. The building is powered by over 1,200 solar photovoltaic panels on its roof, generating more than 500 MWh of electricity annually to achieve a zero or positive energy balance. With a gross floor area of 8,514 square meters, SDE4 houses research laboratories, design studios, and community spaces, fostering interdisciplinary collaboration with public agencies and industry partners. Serving as a living laboratory, it plays a key role in advancing sustainable building technologies.
</figcaption>
</figure>
</div>

<h3 class="research-subtitle">
  <span class="title-line">Smart Green Home</span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/smart_green_home.jpg" alt="Smart Green Home">
</div>

<figcaption class="left-caption">
The Smart Green Home is a cutting-edge indoor test-bed dedicated to advancing research and innovation in smart and sustainable living. This 100 m² full-size home provides a plug-and-play environment for testing smart features, green building technologies, and human-centric design solutions. Its reconfigurable structure enables flexible experimental setups, allowing researchers to study energy efficiency, indoor environmental quality, and sustainable home innovations. The facility also supports the exploration of novel materials, sensor-based control systems, and adaptive facades to enhance occupant comfort while optimizing energy performance.
</figcaption>
</figure>
</div>

<h3 class="research-subtitle">
  <span class="title-line">District cooling systems on campus</span>
</h3>

<div class="research-card-grid">
<figure class="research-card">
<div class="research-card-image-wrap">
<img src="https://maomaohu.net/img/district_cooling_systems.png" alt="District Cooling Systems on Campus">
</div>

<figcaption class="left-caption">
NUS operates multiple district cooling systems that efficiently cool buildings across its campus using centralized chilled water plants. This system produces and distributes chilled water through underground pipes to multiple buildings within a two-kilometer radius, eliminating the need for individual chiller plants and cooling towers. Heat exchangers optimize flow and regulate pressure, improving overall efficiency. By leveraging economies of scale and optimizing asset performance, district cooling reduces energy costs by up to 40% compared to traditional air-conditioning systems. Additionally, it lowers carbon emissions while enhancing grid reliability and climate resilience.
</figcaption>
</figure>
</div>

</main>
</div>

<script>
const sections = document.querySelectorAll(".research-main h2[id], .research-main h3[id]");
const navLinks = document.querySelectorAll(".research-sidebar a");
const sidebarParent = document.querySelector(".sidebar-parent");
const sidebarGroup = document.querySelector(".sidebar-group");

function getOffset() {
  return 110;
}

function setActiveLink() {
  let currentId = "";
  const offset = getOffset();

  sections.forEach(section => {
    const sectionTop = section.offsetTop - offset - 20;
    if (window.scrollY >= sectionTop) {
      currentId = section.getAttribute("id");
    }
  });

  navLinks.forEach(link => {
    link.classList.remove("active");
    if (link.getAttribute("href") === "#" + currentId) {
      link.classList.add("active");
    }
  });

  if (
    currentId === "research-thrusts" ||
    currentId === "free-systems" ||
    currentId === "digitalization" ||
    currentId === "control" ||
    currentId === "ai"
  ) {
    const researchThrustsLink = document.querySelector('.research-sidebar a[href="#research-thrusts"]');

    if (researchThrustsLink) {
      researchThrustsLink.classList.add("active");
    }
  }
}

if (sidebarParent && sidebarGroup) {
  sidebarParent.addEventListener("click", function (e) {
    e.preventDefault();

    const targetId = this.getAttribute("href");
    const targetSection = document.querySelector(targetId);

    sidebarGroup.classList.toggle("open");

    if (targetSection) {
      const offset = getOffset();
      const targetPosition = targetSection.getBoundingClientRect().top + window.pageYOffset - offset;

      window.scrollTo({
        top: targetPosition,
        behavior: "auto"
      });

      history.pushState(null, null, targetId);
    }
  });
}

navLinks.forEach(link => {
  if (link.classList.contains("sidebar-parent")) {
    return;
  }

  link.addEventListener("click", function (e) {
    e.preventDefault();

    const targetId = this.getAttribute("href");
    const targetSection = document.querySelector(targetId);

    if (targetSection) {
      const offset = getOffset();
      const targetPosition = targetSection.getBoundingClientRect().top + window.pageYOffset - offset;

      window.scrollTo({
        top: targetPosition,
        behavior: "auto"
      });

      history.pushState(null, null, targetId);

      navLinks.forEach(item => item.classList.remove("active"));
      this.classList.add("active");

      if (
        targetId === "#free-systems" ||
        targetId === "#digitalization" ||
        targetId === "#control" ||
        targetId === "#ai"
      ) {
        const researchThrustsLink = document.querySelector('.research-sidebar a[href="#research-thrusts"]');

        if (researchThrustsLink) {
          researchThrustsLink.classList.add("active");
        }
      }
    }
  });
});

window.addEventListener("scroll", setActiveLink);
window.addEventListener("load", setActiveLink);
window.addEventListener("resize", setActiveLink);
</script>