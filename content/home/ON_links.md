---
title: 
summary: xxxx
date: 2025-10-22
weight: 140  # Order that this section will appear.

design:
  columns: "1"

# Show estimated reading time?Show social sharing links?Show author profile?Show comments?
reading_time: true
share: true  
profile: true
comments: false
# Optional header image (relative to `static/media/` folder).
# header:  
# caption: ""  
# image: "" 

css_class: "links-section"

---
<div class="links-layout">
  <div class="links-brand">
    <div class="brand-title">
      <span class="brand-nus">NUS</span><span class="brand-divider">|</span><span class="brand-lab">BIOR Lab</span>
    </div>
  <div class="brand-address">
    4 Architecture Drive, #03-04,<br>
    Singapore, 117566<br>
    <a href="https://maomaohu.net/post/post_36_wechat_official/" target="_blank" rel="noopener" style="color:#003D7C; text-decoration:none;">WeChat Official Account</a>
  </div>
  </div>
  <div class="links-columns">
    <div class="links-col">
      <a class="link-text" href="https://www.nus.edu.sg/" target="_blank" rel="noopener">National University of Singapore</a>
      <a class="link-text" href="https://cde.nus.edu.sg/" target="_blank" rel="noopener">College of Design and Engineering</a>
      <a class="link-text" href="https://cde.nus.edu.sg/dbe/" target="_blank" rel="noopener">Department of Built Environment</a>
      <a class="link-text" href="https://cde.nus.edu.sg/dbe/centre-for-digital-building-technology/" target="_blank" rel="noopener">Center for Digital Building Technology (CDBT)</a>
    </div>
    <div class="links-col">
       <a class="link-text" href="https://ai.nus.edu.sg/" target="_blank" rel="noopener">NUS Artificial Intelligence Institute</a>
      <a class="link-text" href="https://esi.nus.edu.sg/" target="_blank" rel="noopener">NUS Energy Studies Institute (ESI)</a>
      <a class="link-text" href="https://iora.nus.edu.sg/" target="_blank" rel="noopener">NUS Institute of Operations Research and Analytics (IORA)</a>
      <a class="link-text" href="https://www.seris.nus.edu.sg/" target="_blank" rel="noopener">NUS Solar Energy Research Institute of Singapore (SERIS)</a>
    </div>
  </div>
</div>
<style>
.links-layout {
  display: grid;
  grid-template-columns: 1.1fr 1.9fr;
  column-gap: 100px;
  align-items: start;
  margin-bottom: 0;
}
.links-brand {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  min-width: 0;
}
.brand-title {
  font-size: 42px;
  line-height: 1.15;
  margin-bottom: 24px;
  word-break: break-word;
}
.brand-nus {
  color: #003D7C;
  font-weight: 700;
}
.brand-divider {
  margin: 0 8px;
  color: #333333;
  font-weight: 400;
}
.brand-lab {
  color: #333333;
  font-weight: 400;
}
.brand-address {
  color: #333333;
  font-size: 18px;
  line-height: 1.5;
  word-break: break-word;
}
.links-columns {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  column-gap: 80px;
  row-gap: 18px;
  align-items: start;
  min-width: 0;
}
.links-col {
  display: flex;
  flex-direction: column;
  gap: 18px;
  min-width: 0;
}
.link-text {
  display: block;
  color: #003D7C;
  text-decoration: none;
  font-size: 18px;
  font-weight: 400;
  line-height: 1.5;
  text-align: left;
  word-break: break-word;
  overflow-wrap: break-word;
}
.link-text:hover {
  text-decoration: underline;
}
.links-brand,
.links-columns,
.links-col {
  margin-bottom: 0;
}
@media (max-width: 900px) {
  .links-layout {
    grid-template-columns: 1fr;
    row-gap: 36px;
    column-gap: 0;
  }
  .links-brand {
    min-height: auto;
  }
  .brand-title {
    margin-bottom: 24px;
    font-size: 32px;
  }
  .links-columns {
    grid-template-columns: 1fr;
    column-gap: 0;
    row-gap: 16px;
  }
  .link-text,
  .brand-address {
    font-size: 17px;
  }
}
.typed-cursor {
  display: none !important;
}
</style>