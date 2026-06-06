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
social: true # includes social icons at the bottom of the page

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

I am an M.S. student in Electrical Engineering at the [Korea Advanced Institute of Science and Technology (KAIST)](https://www.kaist.ac.kr/en/), where I am a member of the [Artificial Intelligence & Machine Learning (U-AIM) Lab](https://sanctusfactory.com/u-aim/) advised by Professor [Chang D. Yoo](https://sanctusfactory.com/family.php). I received my B.S. degree in Smart Vehicle Engineering from Konkuk University.

My research interests lie in multimodal large language models, knowledge distillation, agentic AI, multi-agent systems, and physical AI. Recently, my work has focused on improving the reasoning and visual grounding capabilities of multimodal large language models.

Beyond multimodal language models, I am interested in building AI systems that can interact with complex environments through perception, reasoning, and action. This includes vision-language-action models, embodied AI, and agentic systems that can communicate, refine their decisions, and operate more reliably in real-world scenarios.

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
  min-height: 2rem;
  margin-bottom: 0.75rem;
}

.single-page-tools:empty {
  display: none;
}

.single-page-tools #light-toggle {
  margin: 0;
}

/* Capitalize section headings */
h2 {
  text-transform: capitalize !important;
}
</style>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    var tools = document.querySelector(".single-page-tools");
    var toggle = document.querySelector("#light-toggle");

    if (tools && toggle) {
      tools.appendChild(toggle);
      tools.style.display = "flex";
    }
  });
</script>
