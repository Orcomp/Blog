---
layout : post
title : Good Library Infrastructure
category : Programming
tags :
  - Programming
---

In order to have a good library you need 4 essential ingredients:
1. Good Specifications (or requirements. i.e. Why does this library exist in the first place? What is it trying to solve? Introduce and explain the problem.)
2. Good interface design
3. Unit tests
4. Performance tests

Notice I didn't mention documentation because if you have good specifications, unit tests and a well commented interface you don't need documentation. In other words the documentation should "fall out" of the comments and the specifications.

**Every library should strive to make it easy to**:
- Understand and use.
- Write new implementations (guided by the specifications and unit tests.)
- Compare the performance of a new implementation against existing implementations. (Using already made performance tests, which will automatically compare the new implementation against the existing ones.)

Too often the last 2 points are completely ignored.