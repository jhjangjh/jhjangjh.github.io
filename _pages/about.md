---
layout: about
title: about
permalink: /
subtitle: M.S. Student, Electrical Engineering, KAIST

profile:
  align: left
  image: prof_jaehyun.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>School of Electrical Engineering</p>
    <p>KAIST</p>
    <p>Daejeon, Republic of Korea 🇰🇷</p>

selected_papers: false # publications are rendered below the news section
social: false # social icons are rendered manually in the introduction

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
<div class="single-page-tools" aria-label="Display settings"></div>

<nav class="section-jump-nav" aria-label="Section navigation">
  <a href="#about">About</a>
  <a href="#news">News</a>
  <a href="#education">Education</a>
  <a href="#publications">Publications</a>
  <a href="#projects">Projects</a>
  {% if site.data.honors_awards.size > 0 %}
    <a href="#honors">Honors</a>
  {% endif %}
  {% if site.data.academic_services.size > 0 %}
    <a href="#academic-services">Academic</a>
  {% endif %}
  {% if site.data.teaching_assistant.size > 0 %}
    <a href="#teaching-assistance">TA</a>
  {% endif %}
</nav>

<section id="about" class="profile-section intro-section">

<h2>About</h2>

<p>
  I am an M.S. student in Electrical Engineering at the <a href="https://www.kaist.ac.kr/en/">Korea Advanced Institute of Science and Technology (KAIST)</a>, where I am a member of the <a href="https://sanctusfactory.com/u-aim/">Artificial Intelligence &amp; Machine Learning (U-AIM) Lab</a> advised by Professor <a href="https://sanctusfactory.com/family.php">Chang D. Yoo</a>. I received my B.S. degree in Smart Vehicle Engineering from Konkuk University.
</p>

<p>
  My research focuses on enhancing the visual grounding and reasoning capabilities of Multimodal Large Language Models (MLLMs). Ultimately, I aim to advance <strong>Embodied and Agentic AI systems</strong>—spanning physical, interactive, and multi-agent AI—that bridge the gap between perception and action to operate reliably in complex environments.
</p>

{% include manual_socials.liquid %}

</section>

<style>
/* Hide the navbar for the one-page layout. */
nav.navbar,
.navbar,
.fixed-top {
  display: none !important;
}

body.fixed-top-nav {
  padding-top: 0 !important;
}

.single-page-tools {
  align-items: center;
  display: flex;
  justify-content: flex-end;
  position: fixed;
  right: 1.5rem;
  top: 1rem;
  z-index: 10000;
}

.single-page-tools #light-toggle {
  font-size: 1.25rem;
  height: 2.5rem;
  margin: 0;
  width: 2.5rem;
}

.section-jump-nav {
  border-left: 2px solid var(--global-divider-color);
  display: flex;
  flex-direction: column;
  gap: 0.45rem;
  line-height: 1.2;
  padding-left: 0.9rem;
  position: fixed;
  right: 1.5rem;
  top: 5rem;
  z-index: 9999;
}

.section-jump-nav a {
  color: #667789;
  font-size: 0.92rem;
  font-weight: 700;
  text-decoration: none;
}

.section-jump-nav a:hover {
  color: var(--global-theme-color);
}

/* Capitalize section headings */
h2 {
  text-transform: capitalize !important;
}

.profile-section {
  border-top: 1px solid var(--global-divider-color);
  margin-top: 2rem;
  padding-top: 1.35rem;
  scroll-margin-top: 1.5rem;
}

.intro-section {
  border-top: 0;
  margin-top: 0;
  padding-top: 0;
}

.profile-section h2 {
  margin-top: 0;
}

.intro-section a {
  color: var(--global-theme-color);
  font-weight: 700;
  text-decoration: underline;
  text-underline-offset: 0.16em;
}

.intro-section p {
  margin-bottom: 1rem;
}

@media (max-width: 1200px) {
  .section-jump-nav {
    background: var(--global-bg-color);
    border-bottom: 1px solid var(--global-divider-color);
    border-left: 0;
    border-top: 1px solid var(--global-divider-color);
    align-items: center;
    flex-direction: row;
    gap: 0.8rem;
    left: 0;
    overflow-x: auto;
    padding: 0.55rem 1rem;
    right: 0;
    top: 0;
    white-space: nowrap;
    width: 100%;
  }

  .section-jump-nav a {
    flex: 0 0 auto;
  }

  .single-page-tools {
    align-items: center;
    display: flex !important;
    flex: 0 0 auto;
    order: -1;
    position: static;
  }

  .single-page-tools #light-toggle {
    align-items: center;
    display: inline-flex;
    font-size: 0.95rem;
    height: 1.2rem;
    justify-content: center;
    line-height: 1;
    width: 1.2rem;
  }
}
</style>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    var tools = document.querySelector(".single-page-tools");
    var jumpNav = document.querySelector(".section-jump-nav");
    var toggle = document.querySelector("#light-toggle");
    var mediaQuery = window.matchMedia("(max-width: 1200px)");

    if (tools && toggle) {
      tools.appendChild(toggle);
      tools.style.display = "flex";
    }

    function placeTools() {
      if (!tools || !jumpNav) {
        return;
      }

      if (mediaQuery.matches) {
        jumpNav.insertBefore(tools, jumpNav.firstChild);
      } else {
        document.body.insertBefore(tools, document.body.firstChild);
      }
    }

    placeTools();
    mediaQuery.addEventListener("change", placeTools);
  });
</script>
