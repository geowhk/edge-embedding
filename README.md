# A Typology of School-Age Migration via Edge Representation Learning

**Status:** Conceptual framework for a course-term project.
**Last updated:** Sep 20, 2025

## 1. Abstract

This research proposes a novel framework to create a data-driven typology of school-age migration flows. Traditional migration studies often focus on volumes or individual characteristics, overlooking the rich, contextual nature of the movement itself. By leveraging Edge Representation Learning, this project aims to create vector representations of migration flows that encode the unique attributes of both origins and destinations, enabling a more nuanced understanding of the complex drivers behind educational migration.

## 2. Theoretical Background

The analysis of movement as a distinct entity, rather than just an attribute of a location, has a long tradition in geographic thought. However, quantitative methods have struggled to capture this relational complexity. Recent advancements in graph representation learning, particularly methods that learn embeddings for edges (i.e., relationships) rather than just nodes, offer a powerful new approach. This project specifically draws upon the conceptual foundations of node2vec [1] and other graph embedding techniques to model the directed, heterogeneous nature of migration flows.

## 3. Methodology

1.  **Graph Construction:** A heterogeneous graph will be constructed where nodes represent geographic districts with various attributes (e.g., educational infrastructure, housing prices, demographic data).
2.  **Edge Feature Engineering:** Each migration flow (edge) will be represented as a **dyadic matrix**, capturing the interaction between the feature vectors of the origin and destination nodes. This allows for a rich representation of the relational dynamics (e.g., difference in housing prices, travel distance).
3.  **Edge Embedding:** A state-of-the-art edge embedding algorithm will be employed to generate low-dimensional vector representations for each migration flow.
4.  **Clustering & Interpretation:** Clustering algorithms (e.g., K-Means, HDBSCAN) will be applied to the edge embeddings to identify and interpret distinct migration typologies.

## 4. Expected Contributions

This project is expected to yield a rich, data-driven typology of migration, moving beyond simple volume mapping. Potential typologies to be identified include:

* **'Upward Educational Mobility' flows:** Characterized by movement from areas with lower educational resources to those with significantly higher resources.
* **'Suburban Relocation' flows:** Driven primarily by housing and neighborhood characteristics rather than purely educational factors.
* **'Specialized Program' flows:** Smaller, long-distance flows directed towards specific, unique educational programs.

This novel approach will provide a more granular and context-aware understanding of school-age migration, offering valuable insights for educational policy and urban planning.

## 5. References

[1] Grover, A., & Leskovec, J. (2016). node2vec: Scalable Feature Learning for Networks. *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining.*
