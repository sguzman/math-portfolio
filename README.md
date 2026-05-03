# Math Portfolio

This repository is the top-level map of my mathematical work. It collects a set of specialized repositories and pairs them with portfolio notes that explain what each repo is doing, how the ideas connect, and where the strongest research threads are.

The portfolio is not a single textbook-style project. It is a working research environment spanning exploratory Mathematica notebooks, graph-based whiteboard sketches, mathematical writing, data analysis, and article-scale idea development.

## What this repo is for

- centralize my math-related repositories in one place,
- make exploratory work legible through curated notes,
- preserve connections between raw experiments and higher-level research ideas,
- and provide a readable overview of what I have been trying to build across multiple repos.

## Core research themes

Several themes recur across the portfolio:

- **Iteration as a mathematical object**  
  Repeated function application appears throughout the work, especially as algebra, geometry, operator theory, and Collatz-style dynamics.

- **Curvature, geometry, and shape semantics**  
  Curves, curvature, arc length, and geometric transformations are treated not only visually but as structural carriers of information.

- **Symbolic systems and expression structure**  
  Expressions are often approached as manipulable programs, graph objects, or grammar-like constructions rather than as static notation.

- **Complex numbers and transforms as unifying languages**  
  Complex coordinates, integral transforms, and analytic operators are repeatedly used to reinterpret real-variable behavior.

- **Formalization of intuition**  
  Many repos begin as rough or speculative ideas and gradually move toward more explicit symbolic, computational, or note-based frameworks.

- **Cross-disciplinary mathematical thinking**  
  Some work extends into economics, finance, computation, writing, and philosophy while still being driven by mathematical structure.

## Project map

| Project | Role in the portfolio | Notes |
| :--- | :--- | :--- |
| **[MathematicaMathFun](projects/MathematicaMathFun)** | Largest exploratory math lab; Wolfram Language scripts and notebooks across iteration, Collatz, complex analysis, geometry, transforms, and symbolic experimentation. | [Notes](notes/MathematicaMathFun.md) |
| **[MathWhiteBoard](projects/MathWhiteBoard)** | Visual scratchpad for modeling mathematical expressions as graphs and studying normalization through structure. | [Notes](notes/MathWhiteBoard.md) |
| **[Math Research](projects/math-research)** | Curated research directions and paper-scale work, including PDFs tied to iteration and process-oriented themes. | [Notes](notes/math-research.md) |
| **[Mathematica Data](projects/mathematica-data)** | Data-oriented Mathematica work focused on economic indicators, correlations, and structured datasets. | [Notes](notes/mathematica-data.md) |
| **[TS-Mathematica](projects/ts-mathematica)** | Hybrid TypeScript and Wolfram work, especially around statistical and financial analysis. | [Notes](notes/ts-mathematica.md) |
| **[Articles](projects/articles)** | Writing repo for treatises, math idea backlogs, research agendas, and conceptual material that sits above the code-heavy repos. | [Notes](notes/articles.md) |

## How the pieces fit together

This portfolio has a deliberate split between **raw work** and **explanatory work**:

- `projects/` contains the original repositories as submodules.
- `notes/` contains portfolio-side documentation that explains what those repos are doing.

That distinction matters because many source repos are exploratory by design. Their internal filenames, notebooks, or scratch scripts are often meaningful to me in context, but not automatically legible to someone approaching the work from outside. The notes layer is where I translate raw exploration into a more coherent map.

In practice:

- `MathematicaMathFun` contains the densest mathematical experimentation.
- `MathWhiteBoard` captures structural and graph-based intuition.
- `math-research` and `articles` capture the agenda-setting and article-level side of the work.
- `mathematica-data` and `ts-mathematica` show more applied and computational branches.

## Reading guide

If you want the shortest path through the portfolio, start here:

1. Read `notes/MathematicaMathFun.md` for the main computational research program.
2. Read `notes/articles.md` and `notes/articles/math.md` for the high-level idea backlog and mathematical worldview behind the experiments.
3. Read `notes/math-research.md` for paper-scale direction.
4. Read `notes/MathWhiteBoard.md` for expression-graph and normalization work.
5. Read the applied notes in `notes/mathematica-data.md` and `notes/ts-mathematica.md` for the data-analysis side.

## Repo structure

- `projects/`: git submodules for the underlying repositories.
- `notes/`: curated explanations, summaries, and thematic expansions.
- `tmp/`: local scratch space for temporary work in this portfolio repo.

## Working style

The portfolio reflects a specific way of doing mathematical work:

- start with an intuition, question, or symbolic pattern,
- test it computationally, often in Wolfram Language,
- split the idea into multiple small files or variants,
- preserve both successful and failed branches,
- then document the pattern afterwards in notes.

This means the repos are not uniformly polished. Some are close to research notebooks, some are closer to conceptual archives, and some are clearly structured subprojects. The value of the portfolio is in preserving the full research trail while making it interpretable.

## Tooling and mediums

The main tools used across the portfolio are:

- **Wolfram Mathematica / Wolfram Language** for symbolic computation, plotting, transforms, geometry, and data work.
- **Markdown** for explanatory notes, research backlogs, and writing.
- **Graphviz / DOT-style graph outputs** for expression and structure visualization.
- **TypeScript** in the mixed computational repos where typed tooling supports mathematical workflows.

## What is documented here

The top-level notes are intended to do more than summarize filenames. They aim to identify:

- the dominant mathematical questions in each repo,
- the internal categories of work,
- the relationship between computational experiments and broader research goals,
- and the conceptual links between separate repositories.

That is especially important for the larger repos, where the raw source material is too broad or too informal to be self-explanatory.

## Current emphasis

At the current stage, the strongest documented emphasis is on:

- iterative dynamics and functional calculus,
- Collatz and grammar-like reformulations,
- curvature and geometric semantics,
- complex-number representations of real behavior,
- transform-based analysis,
- and mathematical writing that extracts broader theory from exploratory computation.

## Notes index

- `notes/MathematicaMathFun.md`
- `notes/MathWhiteBoard.md`
- `notes/math-research.md`
- `notes/mathematica-data.md`
- `notes/ts-mathematica.md`
- `notes/articles.md`
- `notes/articles/math.md`

## Status

This is a living portfolio. It is expected to expand as additional repositories, raw files, and notes are incorporated. The documentation layer is meant to keep pace with that growth so the overall body of work remains navigable.
