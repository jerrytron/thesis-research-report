---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Immersive Tool Design
layout: splash
#layout: home
author_profile: true

classes:
    - landing
excerpt: 'Welcome! My name is Jerry Belich, an experimental game and experience designer. This website is meant to provide an overview of the research I performed for my thesis in pursuit of my MFA in Experience Design at Miami University which I completed in the Spring of 2019.<br />'
header:
    overlay_color: "#333"
    overlay_image: /assets/images/home-banner.png
    overlay_filter: rgba(0, 0, 0, 0.35)
    caption:
    actions:
      - label: "The Research Report"
        url: "/report/01-background/"

feature_row:
  - image_path: /assets/images/feature-xd.png
    alt: "experience design"
    title: "Experience Design"
    excerpt: "This site was created by a graduate of Miami University's Experience Design MFA to summarize their thesis design research."
    url: "http://xd.miamioh.edu/"
    btn_label: "Learn More"
    btn_class: "btn--warning"
  - image_path: /assets/images/feature-web.png
    alt: "jekyll"
    title: "Jekyll"
    excerpt: "Jekyll is a simple, blog-aware, static site generator. It spits out a ready-to-publish static website suitable for serving with your favorite web server."
    url: "http://jekyllrb.com/"
    btn_label: "Learn More"
    btn_class: "btn--success"
  - image_path: /assets/images/feature-theme.png
    alt: "minimal mistakes"
    title: "Minimal Mistakes"
    excerpt: "This theme was built on HTML5 + CSS3. All layouts are fully responsive with helpers to augment your content. 100% free and MIT licensed."
    url: "https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/"
    btn_label: "Learn More"
    btn_class: "btn--info"
intro:
  - excerpt: 'Follow me and my work &nbsp;[<i class="fab fa-fw fa-twitter-square"></i> @j3rrytron](https://twitter.com/j3rrytron){: .btn .btn--twitter} &nbsp; [<i class="fas fa-fw fa-link"></i> jerrytron.com](http://jerrytron.com){: .btn .btn--success}'
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}