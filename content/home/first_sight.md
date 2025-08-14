
---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/getting-started/page-builder/
widget: blank
active: true
headless: true
weight: 15

title: 
subtitle:

design:
  columns: "1"
  background:
    image: web_first_sight_4.png
    image_darken: 0.1
    image_parallax: false
    image_position: center
    image_size: cover
    text_color_light: true
  spacing:
    padding: ["0px", "0px", "0px", "0px"]   # Order is top, right, bottom, left.

advanced:
   css_style: "min-height: calc(100vh + 10px); margin-top: -10px; padding-top: 10px; display:flex; align-items:center; justify-content:center;"
---

<font size="6">Building Informatics and Operations Research (BIOR) Lab</font>

<font size="6">National University of Singapore</font>

<style>
  code {
    background: none !important;
    border: none !important;
    padding: 0;
    box-shadow: none !important;
  }
</style>

<div style="text-align: left; font-size: 22px;">
  <code style="color: #FFFFFF">Smart Decisions for </code>
  <div id="typed-strings">
    <p ><code style="color: #EF7C00; font-weight: bold;">Smart</code></p>
    <p ><code style="color: #EF7C00; font-weight: bold;">Low-carbon</code></p>
    <p><code style="color: #EF7C00; font-weight: bold;">Energy-efficient</code></p>
    <p><code style="color: #EF7C00; font-weight: bold;">Demand-flexible</code></p>
    <p><code style="color: #EF7C00; font-weight: bold;">Climate-resilient</code></p>
    <p><code style="color: #EF7C00; font-weight: bold;">Equitable</code></p>
  </div>
  <span class="font-bold" id="typed"></span>
  <code style="color: #FFFFFF">&nbsp;Building, District, and Urban Energy Systems.</code>
</div>

<!-- Include Typed.js -->
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
