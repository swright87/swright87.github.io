---
layout: about
title: About
permalink: /
subtitle: <a href='#'>Reader in Computer Science</a>. University of York.

profile:
  align: right
  image: profile_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>CSE/135</p>
    <p>Computer Science</p>
    <p>University of York</p>
    <p>YO10 5GH, UK</p>
    <p>Phone: +44 (0)1904 325583</p>

selected_papers: false # the layout's own hard-coded "selected publications" heading;
# off so the heading below can be written in the page body instead
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: false # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: false # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a Reader in [Computer Science at the University of York](https://www.cs.york.ac.uk), having joined the department in July 2018. I am a member of the [Real-Time and Distributed Systems](https://www.cs.york.ac.uk/research/groups/real-time-distributed-systems/) research group. My research is broadly focussed on **High Performance Computing**, in particular looking at the performance, programmability, and energy efficiency of supercomputers and the scientific computing applications running on them. Throughout my career I have collaborated widely with colleagues from national laboratories, universities and industry, including the US Department of Energy, the UK Atomic Energy Authority, the York Plasma Institute, Rolls-Royce, Intel, NVIDIA, ARM, and IBM.

Prior to joining York, I was a Research Fellow within the [High Performance and Scientific Computing (HPSC)](https://warwick.ac.uk/fac/sci/dcs/research/dsss/) research group at the University of Warwick, working on projects with the [Centre for Fusion, Space and Astrophysics](https://warwick.ac.uk/fac/sci/physics/research/cfsa/), Sandia National Laboratories, and Rolls-Royce. I completed my Ph. D. at Warwick in 2014 with a thesis titled "Monitoring, Analysis and Optimisation of I/O in Parallel Applications".

I co-chair the [International Workshop on Performance Modeling, Benchmarking and Simulation of High Performance Computer Systems (PMBS)](https://pmbs-workshop.github.io), held annually at ACM/IEEE Supercomputing, and have edited its proceedings every year since 2013. I am also an author on the third edition of Pacheco's [_An Introduction to Parallel Programming_]({{ '/book/' | relative_url }}) (Morgan Kaufmann), due out in December 2026.

At York I have taught across the degree programme, and I currently serve as the Chair of the Board of Examiners. I currently lead the [High-Performance Parallel and Distributed Systems (HIPC)](https://www.york.ac.uk/students/studying/manage/programmes/module-catalogue/module/COM00036H/latest/) module, and previously led the [Software Testing (SOTE)](https://www.york.ac.uk/students/studying/manage/programmes/module-catalogue/module/COM00122M/latest/) module. While at Warwick, I led the [Programming for Computer Scientists (CS118)](https://warwick.ac.uk/fac/sci/dcs/teaching/modules/cs118/) module.

<div style="clear: both; display: flex; gap: 1.25rem; align-items: center; margin: 2rem 0; padding: 1rem 1.25rem; border: 1px solid var(--global-divider-color); border-left: 4px solid var(--global-theme-color); border-radius: 6px;">
  <a href="{{ '/book/' | relative_url }}" style="flex: 0 0 auto;">
    <img
      src="{{ 'assets/img/ipp-wright-book.png' | relative_url }}"
      alt="Cover of An Introduction to Parallel Programming, Third Edition"
      style="width: 80px; height: auto; border-radius: 3px; box-shadow: 0 2px 8px rgba(0, 0, 0, 0.25);"
    >
  </a>
  <div>
    <div style="font-size: 0.8rem; font-weight: 700; letter-spacing: 0.05em; text-transform: uppercase; color: var(--global-theme-color);">
      New book &middot; December 2026
    </div>
    <div style="font-size: 1.15rem; font-weight: 600; margin: 0.25rem 0;">
      <a href="{{ '/book/' | relative_url }}" style="color: inherit;">An Introduction to Parallel Programming</a>, Third Edition
    </div>
    <div style="margin-bottom: 0.4rem;">
      Peter S. Pacheco, Matthew Malensek, and <a>Steven A. Wright</a>.
    </div>
    <a href="{{ '/book/' | relative_url }}">About the book</a> &middot;
    <a href="https://shop.elsevier.com/books/an-introduction-to-parallel-programming/wright/978-0-443-36702-1">Order from Elsevier &rarr;</a>
  </div>
</div>

## Selected Publications

{% include selected_papers.liquid %}
