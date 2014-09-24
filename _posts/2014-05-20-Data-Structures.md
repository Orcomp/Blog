---
layout : post
title : Data Structures
category : Programming
tags :
  - Data Structures
  - Algorithms
---

The aim of this post is to collect ideas in order to create an open source (MIT) library of data structures.

A lot of emphasis will be placed on performance and structure (Interface).

The library will come with a suite of unit and performance tests which will target the interface.

Low barrier to implementation.
Allow people to write their own implementation with ready made unit and performance tests they can check their work against.

Namespaces:
- DS.Interfaces
- DS.Core
- DS.Trees
- DS.Graphs
- DS.Intervals

(Other datastructures to consider, ordered Set, Pascal Set)

Performance tests will be written against the interface using [NUnitBenchmarker](https://github.com/Orcomp/NUnitBenchmarker). This will allow us to write performance tests once and then run the performance tests against many implementations.

We will look for the existing best open source implementations and include them (with proper reference) in the library.


## DS.Trees

The trees I am interested in are:
- Andersson Trees
- AVL Trees
- BTree
- Binary Search Trees
- Hash Tables
- Red Black Trees
- Skip Lists


# Links:

- Excellent introduction to various tree data structures: http://www.eternallyconfuzzled.com/tuts/datastructures/jsw_tut_andersson.aspx
- http://msdn.microsoft.com/en-au/library/ms379570(v=vs.80).aspx
- http://www.codeproject.com/Articles/274486/A-Better-Sorted-List-and-Dictionary
- http://www.codeproject.com/Articles/610399/SortedSplitList-An-Indexing-Algorithm-in-Csharp

# Implementations

|Link| Language| License| Trees | Notes
|[C5](https://github.com/sestoft/C5)| C# | BSD | Red Black
|[PowerCollection](https://powercollections.codeplex.com/)|C#|EPL|
|[adjunct](https://adjunct.codeplex.com)|C#|MS-PL| AVL, Binary | Look in the source
|[vds-common](https://bitbucket.org/rvesse/vds-common)|C#|MIT| AVL, Scapegoat, Unbalanced
|[AATree Implementation](http://demakov.com/snippets/aatree.html)|C#|??| Andersson Tree
|[AList](http://www.codeproject.com/Articles/568095/The-List-Trifecta-Part)|C#|LGPL v3|








