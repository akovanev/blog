---
title: "Visualize project planning and execution"
categories:
  - Project Management
tags:
  - excalidraw
---

Although many tracking tools and various plugins help visualize dependencies between tasks, they often come with drawbacks such as requiring payment, lacking essential features, or having an unattractive UI.

In the projects I lead, I prefer using a tool called [Excalidraw](https://excalidraw.com). While it is just a board, I find it great for illustrating dependencies and the current state of the project.

Here is a simple example of planning the delivery of a new microservice to staging. Different colors distinguish the work areas.

<a href="{{ site.url }}{{ site.baseurl }}/assets/images/ex-plan.png"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/ex-plan.png" /></a>

I use an approach similar to [Petri nets](https://en.wikipedia.org/wiki/Petri_net#:~:text=A%20Petri%20net%2C%20also%20known,of%20elements%3A%20places%20and%20transitions), where tasks represent places and transitions indicate the work that must be completed before moving to the next step.

<a href="{{ site.url }}{{ site.baseurl }}/assets/images/ex-work.png"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/ex-work.png" /></a>

New issues can be added during the process. The current state is determined by the filling type, allowing you to see the progress at any point. Additionally, you might include helpful information to align the work.