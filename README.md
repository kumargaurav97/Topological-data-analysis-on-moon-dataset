# Topological-data-analysis-on-moon-dataset
use the gudhi library 
Homology is a concept from algebraic topology that measures the shape of a space — more specifically, it detects holes of different dimensions.
H0 features = connected components

H1 features = loops (e.g., the "hole" in a donut)

H2 features = voids (like inside a sphere)
TDA uses homology to study the structure of data, even if it’s high-dimensional or noisy.

A Rips complex (or Vietoris–Rips complex) is a way to approximate the shape of a dataset (point cloud) using simplices (generalizations of triangles):

You start with a bunch of points.

For a given distance threshold ε:

Connect two points with an edge if they are ≤ ε apart.

Add a triangle if all three pairwise distances are ≤ ε.

Add higher-dimensional simplices similarly.

This gives a combinatorial object (a simplicial complex) that captures the data’s structure.
In real data, the shape depends on the scale — if points are too far apart, you miss connections; too close, and you connect everything.

Persistent homology analyzes how the topological features (like loops, voids, clusters) persist as you vary the scale.
