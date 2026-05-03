# Math Portfolio

This repository is a map of my mathematical research areas. The point is not just to collect repositories, but to make legible the raw lines of thought running through them: iteration, curvature, symbolic structure, topology, analytic transforms, and the attempt to build better formalisms for mathematical intuition.

Much of the work is exploratory. Some parts are computational, some are visual, some are article-scale, and some are only partially formalized. What unifies them is the attempt to treat mathematics as a live research process rather than a finished archive.

## Main research areas

### Iteration, dynamics, and Collatz

One of the strongest recurring themes is repeated function application. I am interested in iteration not only as a discrete process, but as something that should admit its own algebra, geometry, and operator theory.

This includes:

- Collatz-style dynamics and orbit behavior,
- fractional or continuous versions of iteration,
- function application as an analytic object,
- operator-theoretic views of state evolution,
- and symbolic or grammar-based reformulations of iterative systems.

The broader goal is to turn “apply this function again” into something mathematically manipulable in its own right.

### Curvature, geometry, and shape semantics

Another major area is the idea that curves carry semantic structure. Curvature is not just a geometric statistic here; it is often treated as information, control, or evidence of how a function is built.

This includes:

- curvature and arc-length analysis,
- parametric curves and geometric deformation,
- line-versus-curve comparisons,
- Euclidean operations as analyzable primitives,
- and the idea that complicated shapes may become simple in the right space.

The recurring instinct is that geometry can explain symbolic behavior, not merely illustrate it.

### Complex numbers and analytic representation

Complex numbers appear throughout the work as a unifying language for dynamics and geometry. They are used not only in a classical complex-analysis sense, but as a compact representation for rotation, scaling, curvature, and iterative behavior.

This includes:

- polar and complex encodings of real phenomena,
- holomorphic viewpoints on real-variable iteration,
- domain-coloring and visualization-driven analysis,
- and attempts to decompose real curves into complex-valued structure.

The underlying question is whether complex language is not just useful, but the right representation for phenomena that look harder in purely real coordinates.

### Symbolic structure, expressions, and algebraic computation

A large part of the portfolio treats expressions as structured computational objects. Algebra is often approached operationally: equations, expressions, and transforms are things to manipulate, normalize, compress, or reinterpret.

This includes:

- expressions as programs,
- normal forms and symbolic compression,
- algebraic objects as compositional structures,
- graph-based representations of expressions,
- and mathematical syntax as a carrier of execution semantics.

This is one of the main bridges between the computational work and the more philosophical writing.

### Topology, homotopy, and ambient-space reasoning

There is also a persistent topological thread. The focus is less on textbook coverage and more on how connectedness, holes, boundaries, neighborhoods, and deformation can be used to reason about mathematical and symbolic objects.

This includes:

- homotopy as interpolation and transformation,
- boundary behavior under equivalence,
- connectedness versus homology,
- ambient-space methods for studying structure,
- and questions about when interpolation preserves deeper structure.

The common pattern is to ask when geometric deformation preserves identity and when it changes the object in a deeper way.

### Integral transforms, convolution, and structural probes

Transforms often appear as instruments for extracting hidden behavior. Convolution, Laplacians, Dirac delta methods, and integral transforms are treated as ways to interrogate functions rather than merely rewrite them.

This includes:

- convolution as scanning or local action,
- transforms as property detectors,
- Laplacian-driven deformation,
- zero-detection and localization methods,
- and the idea of integral machinery as a general-purpose analysis framework.

The deeper research instinct is that a good transform should expose structure that is otherwise difficult to see directly.

### Alternative spatial and algebraic representations

Some work tries to redesign the underlying representation altogether. Instead of assuming standard coordinates, standard matrices, or standard geometric primitives are enough, the portfolio repeatedly experiments with alternative encodings.

This includes:

- representing curves as boolean or matrix-valued fields,
- using infinite ambient matrices with zero-fill semantics,
- relativizing `R^2` against a chosen reference curve,
- alternative coordinate systems based on dot products or relational structure,
- and interface-inspired operations such as scrolling or moving through mathematical space.

This area is exploratory, but it matters because it reflects a deeper belief that better representations can simplify harder mathematics.

### Meta-mathematics and research methodology

Not all of the work is about solving isolated problems. Some of it is about what mathematical formalisms are for, how they should be judged, and how intuition becomes tractable theory.

This includes:

- measuring the health of a formalism by the problems it can absorb,
- the tradeoff between expressive power and tractability,
- symbol fatigue and math anxiety,
- the relation between structure and dynamics,
- and the idea that some problems require formalisms with enough “infinity” built into them.

This is the most reflective layer of the portfolio and explains why the raw work often moves between computation, notation, and conceptual writing.

## How the work is expressed

The research appears in several different forms:

- computational experiments, mainly in Wolfram Language,
- visual models of expressions and transformations,
- mathematical notes and research backlogs,
- article and treatise drafts,
- and smaller applied studies involving data, finance, or statistical modeling.

That variety is intentional. Some ideas are easiest to discover computationally, some visually, and some only after they are rewritten in prose.

## Portfolio structure

The repositories in `projects/` are the raw working sources. The notes in `notes/` are the explanatory layer that turns those sources into a readable research map.

Current projects:

- `projects/MathematicaMathFun`
- `projects/MathWhiteBoard`
- `projects/math-research`
- `projects/mathematica-data`
- `projects/ts-mathematica`
- `projects/articles`

Current top-level notes:

- `notes/MathematicaMathFun.md`
- `notes/MathWhiteBoard.md`
- `notes/math-research.md`
- `notes/mathematica-data.md`
- `notes/ts-mathematica.md`
- `notes/articles.md`
- `notes/articles/math.md`

## Reading guide

If you want the clearest overview of the mathematical content, start with:

1. `notes/MathematicaMathFun.md`
2. `notes/articles.md`
3. `notes/articles/math.md`
4. `notes/math-research.md`

Then use the project repos as the raw source layer behind those summaries.

## Status

This is a living research portfolio. More repositories, notes, and raw files will be added over time. The aim is to preserve the exploratory character of the work while making the overall mathematical program increasingly explicit.
