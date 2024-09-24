---
title: "Shaping or Foundation first"
categories:
  - Project Management
---

Some time ago we started planning a new microservice with several complex functions. Ideally, we would shape the service first, present the architecture, align it with all involved teams, and then move to implementation.

In theory, this sequence - shaping first, implementation second - makes sense. However, with 3 or even 4 teams playing this game together, there were many unknowns at the beginning. To avoid delays in future, we decided to start building the foundation before all the details were finalized.

The idea was straightforward: we would set up the development and staging infrastructure early on, making it convenient for the development process. Once the shaping and design phases were clarified and approved, we would be ready with everything in place for next delivery.

Naturally, starting without full clarity meant being prepared for rework. And that happened to us. From the outset, we were not sure whether we needed a NoSQL database, cache, or both. So, we decided to create infrastructure for both storages and run some tests to ensure everything worked as expected.

As we progressed with shaping, it became clear that, given the specifics of the service, we didn’t need NoSQL and could rely on caching alone. This led to the removal of all infrastructure and code related to the NoSQL setup.

In total, we spent around 45 man-hours creating and then removing that part of the infrastructure — spread across multiple tasks, but still significant.

Looking back on this experience, my thoughts can be summarized as follows:

* The number of meetings we had to go through during the shaping phase was huge, and the alignment process took a long time. We chose to prepare one of the most complicated parts early on, and I believe that if we hadn't started this way, we wouldn't be ready for the next steps now. While we did spend those hours, the alternative would have been just waiting and accomplishing nothing.

* During this period, we learned a lot about our infrastructure, and the process was also helpful for new people joining the project.

Overall, I consider this experience a positive one. It would be great to gather even more insights on this topic in the future.