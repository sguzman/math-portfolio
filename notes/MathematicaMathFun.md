# MathematicaMathFun

`projects/MathematicaMathFun` is the largest exploratory repository in this portfolio. It is a working lab of Wolfram Language scripts and notebooks rather than a polished single-project codebase. The dominant pattern is iterative mathematical experimentation: define an idea, push it through symbolic algebra or visualization, then branch into adjacent files as the idea changes.

## Scope and structure

- **Primary medium**: Wolfram Language scripts (`.wls`) with a smaller set of Mathematica notebooks (`.nb`).
- **Scale**: about `128` script files and `3` notebook files, plus two notebook-format files saved with a `.wls` extension: `projects/MathematicaMathFun/wls/connections.wls` and `projects/MathematicaMathFun/wls/math.wls`.
- **Layout**:
  - `projects/MathematicaMathFun/` contains a few top-level scripts and notebooks.
  - `projects/MathematicaMathFun/wls/` contains the main body of the work.
- **Duplicate files**: the top level mirrors a few files also present in `wls/`: `calculus-of-var.wls`, `complex-fun.wls`, `curvy-curves.wls`, `just_some_fun.wls`, `pie-charts.wls`, and `stats.wls`.

## What the repo is about

This repo is best understood as a set of connected research threads:

1. **Iteration as algebra and geometry**  
   A large portion of the repo studies repeated function application, fractional or generalized iteration, and ways to reinterpret iteration as rotation, linear transformation, graph structure, or complex multiplication.

2. **Collatz and grammar-based dynamics**  
   Another major thread recasts Collatz-style processes as rewrite systems, parity grammars, and state machines. Several files are clearly successive versions of the same idea rather than separate projects.

3. **Complex numbers as a language for dynamics**  
   Many scripts try to understand functions, derivatives, transforms, and iteration through complex coordinates, polar form, domain coloring, and geometric decompositions into magnitude and angle.

4. **Geometry, curvature, and variational calculus**  
   There is a strong secondary theme around parametric curves, curvature, arc length, Frenet-style analysis, and classical symbolic calculus tools such as Laplace transforms and Euler-Lagrange style questions.

5. **Data, economics, and finance**  
   A separate cluster uses Mathematica's data sources for GDP, inflation, market prices, sector breakdowns, and company or administrative-division metadata.

6. **Open-ended scratch work**  
   Many files are genuine exploratory notebooks in script form. The filenames and opening cells show that they are short experiments, derivation fragments, or checkpoints in longer lines of thought.

## Main research threads

### Iteration, functional calculus, and dynamical systems

This is the center of gravity of the repo. The recurring idea is that function iteration is not treated only as repeated substitution; it is treated as an algebraic object with its own geometry. The work moves between symbolic identities, visual intuition, and alternative encodings.

- **Rotation / geometric models of iteration**: `projects/MathematicaMathFun/wls/iteration_as_rotation.wls`, `projects/MathematicaMathFun/wls/iteration_rotation.wls`, `projects/MathematicaMathFun/wls/iterated-rotation-success.wls`, `projects/MathematicaMathFun/wls/iteration_finished.wls`, `projects/MathematicaMathFun/wls/iter_as_matrix_rotation.wls`, `projects/MathematicaMathFun/wls/iter_as_complex_1.wls`
- **Linear / algebraic formulations**: `projects/MathematicaMathFun/wls/iteration_as_linear_trans.wls`, `projects/MathematicaMathFun/wls/iterate_algebra.wls`, `projects/MathematicaMathFun/wls/iteration_as_complex_algebra.wls`, `projects/MathematicaMathFun/wls/iterated_arith_as_complex_num.wls`, `projects/MathematicaMathFun/wls/iterated_coefficients.wls`
- **Generalized and analytic iteration**: `projects/MathematicaMathFun/wls/iterated_calculus.wls`, `projects/MathematicaMathFun/wls/iterate_my_func.wls`, `projects/MathematicaMathFun/wls/real_iteration.wls`, `projects/MathematicaMathFun/wls/series-iter.wls`, `projects/MathematicaMathFun/wls/iterate_my_func.wls`
- **Supporting representations**: `projects/MathematicaMathFun/wls/iteration_as_graph.wls`, `projects/MathematicaMathFun/wls/complex-iter-fun.wls`, `projects/MathematicaMathFun/wls/gen-funcs.wls`, `projects/MathematicaMathFun/wls/fix_comp.wls`, `projects/MathematicaMathFun/wls/found-it.wls`, `projects/MathematicaMathFun/wls/flumoxed-and-blocked.wls`, `projects/MathematicaMathFun/wls/i-did-it.wls`, `projects/MathematicaMathFun/wls/i-figured-it-out-i-was-right.wls`, `projects/MathematicaMathFun/wls/i_fought_the_math_and_the_math_won.wls`, `projects/MathematicaMathFun/wls/idk_what_im_doing.wls`

Interpretation: this thread is trying to build a calculus of iteration, not just isolated numerical examples.

### Collatz, parity logic, grammars, and rewrite systems

This thread is the other large coherent block. The common move is to encode the Collatz map, parity behavior, or recursive arithmetic into symbolic languages and grammar rules.

- **Base Collatz implementations and templates**: `projects/MathematicaMathFun/wls/collatz_template.wls`, `projects/MathematicaMathFun/wls/collatz-op.wls`, `projects/MathematicaMathFun/wls/collatz-log-counting.wls`, `projects/MathematicaMathFun/wls/collatz_log_stuff.wls`, `projects/MathematicaMathFun/wls/log-props.wls`, `projects/MathematicaMathFun/wls/more_collatz_and_analysis.wls`
- **Grammar construction and revision cycle**: `projects/MathematicaMathFun/wls/collatz_grammar_almost_done.wls`, `projects/MathematicaMathFun/wls/collatz_grammar_fix_this.wls`, `projects/MathematicaMathFun/wls/collatz_grammar_methods_perfected.wls`, `projects/MathematicaMathFun/wls/collatz_grammar_new_rules.wls`, `projects/MathematicaMathFun/wls/grammar_but_it_doesnt_end.wls`, `projects/MathematicaMathFun/wls/grammar_deconstruction.wls`, `projects/MathematicaMathFun/wls/grammar_fun.wls`, `projects/MathematicaMathFun/wls/grammar_minimal.wls`, `projects/MathematicaMathFun/wls/grammar_new_measure_metric.wls`, `projects/MathematicaMathFun/wls/grammar_stuff.wls`, `projects/MathematicaMathFun/wls/grammars_build_up.wls`, `projects/MathematicaMathFun/wls/grammatical_stuff.wls`, `projects/MathematicaMathFun/wls/i_am_a_grammarian_now.wls`, `projects/MathematicaMathFun/wls/enough_grammars_for_now.wls`
- **Automata, limits, and proof attempts**: `projects/MathematicaMathFun/wls/iteration_as_FSM.wls`, `projects/MathematicaMathFun/wls/lang_id_at_limit.wls`, `projects/MathematicaMathFun/wls/odd_even_odd_eq_proof.wls`, `projects/MathematicaMathFun/wls/trees.wls`, `projects/MathematicaMathFun/wls/tick_tock.wls`, `projects/MathematicaMathFun/wls/discrete-alge.wls`, `projects/MathematicaMathFun/wls/int-trans-logic.wls`, `projects/MathematicaMathFun/wls/backtomath.wls`, `projects/MathematicaMathFun/wls/proofs_and_stuff.wls`

Interpretation: this is not just Collatz computation; it is an attempt to formalize parity-driven iteration as a symbolic system with compositional rules.

### Complex numbers, transforms, and analytic visualization

This thread studies complex numbers both directly and as a modeling language for iteration and transformation. The opening cells show repeated use of `ComplexPlot`, polar coordinates, `TrigToExp`, `ReIm`, and symbolic conversions between algebraic and geometric descriptions.

- **Core complex exploration**: `projects/MathematicaMathFun/wls/complex-fun.wls`, `projects/MathematicaMathFun/wls/complex-fun2.wls`, `projects/MathematicaMathFun/wls/complex_nums.wls`, `projects/MathematicaMathFun/wls/complex_nums_to_iter_unc.wls`, `projects/MathematicaMathFun/wls/what_even_are_complex_nums.wls`, `projects/MathematicaMathFun/wls/i_finally_understand_complex_nums.wls`, `projects/MathematicaMathFun/wls/I_am_satisfied_with_complex_stuff.wls`
- **Visualization-heavy scripts**: `projects/MathematicaMathFun/wls/complex_plots.wls`, `projects/MathematicaMathFun/wls/complex_visual.wls`, `projects/MathematicaMathFun/wls/a_complex_story.nb`, `projects/MathematicaMathFun/wls/connections.wls`
- **Polar / decomposition viewpoints**: `projects/MathematicaMathFun/wls/comp.wls`, `projects/MathematicaMathFun/wls/comp-ops.wls`, `projects/MathematicaMathFun/wls/decompose_into_len_and_rot.wls`, `projects/MathematicaMathFun/wls/func_as_complex_rot.wls`, `projects/MathematicaMathFun/wls/oh-well.wls`, `projects/MathematicaMathFun/wls/why-isnt-it-working.wls`
- **Transforms and analytic operators**: `projects/MathematicaMathFun/wls/laplace.wls`, `projects/MathematicaMathFun/wls/laplace-again.wls`, `projects/MathematicaMathFun/wls/disc-ztr.wls`, `projects/MathematicaMathFun/wls/log-zeta.wls`, `projects/MathematicaMathFun/wls/what_am_i_even_doing.wls`, `projects/MathematicaMathFun/wls/mathy-stuff.wls`, `projects/MathematicaMathFun/wls/maybe-fourier.wls`, `projects/MathematicaMathFun/wls/power-of-my-waves.wls`, `projects/MathematicaMathFun/wls/signal-stugff.wls`, `projects/MathematicaMathFun/wls/systems-op.wls`

Interpretation: this branch uses complex analysis less as a formal textbook sequence and more as a unifying representation for dynamic and symbolic phenomena.

### Geometry, curvature, variation, and continuous analysis

Several files focus on curves, curvature, arc length, and symbolic differential analysis. These tend to work through parametrized examples and compare alternate coordinate descriptions.

- **Curves and curvature**: `projects/MathematicaMathFun/curvy-curves.wls`, `projects/MathematicaMathFun/wls/back_to_geo.wls`, `projects/MathematicaMathFun/wls/curvature_analysis.wls`, `projects/MathematicaMathFun/wls/curvature_vs_dot_dir.wls`, `projects/MathematicaMathFun/wls/contours-of-life.wls`, `projects/MathematicaMathFun/math_and_stuff.wls`
- **Calculus of variations and differential equations**: `projects/MathematicaMathFun/calculus-of-var.wls`, `projects/MathematicaMathFun/wls/calculus-of-var.wls`, `projects/MathematicaMathFun/wls/variation.wls`, `projects/MathematicaMathFun/wls/random_math_stuff_idk.wls`, `projects/MathematicaMathFun/wls/jordan-decomp.wls`
- **Spectral / harmonic geometry**: `projects/MathematicaMathFun/wls/spectral_theory.wls`, `projects/MathematicaMathFun/wls/x-exp.wls`, `projects/MathematicaMathFun/wls/studying-polys.wls`

Interpretation: this thread is concerned with how local differential information becomes visible as shape, oscillation, or symbolic structure.

### Algebra, polynomials, number patterns, and symbolic structure

Some scripts are centered less on dynamics and more on algebraic identities, polynomial behavior, combinatorics, and symbolic experimentation.

- **Polynomial and algebraic experiments**: `projects/MathematicaMathFun/wls/alge-bruh.wls`, `projects/MathematicaMathFun/wls/algebra_as_straight_edge_and_compass.wls`, `projects/MathematicaMathFun/wls/more-poly-stuff.wls`, `projects/MathematicaMathFun/wls/poly-fun.wls`, `projects/MathematicaMathFun/wls/studying-polys.wls`, `projects/MathematicaMathFun/wls/theres-something-about-polynomials.wls`
- **Arithmetic / irrational / symbolic themes**: `projects/MathematicaMathFun/wls/irrational_nums.wls`, `projects/MathematicaMathFun/wls/eveness_measure.wls`, `projects/MathematicaMathFun/wls/evenness-measure2.wls`, `projects/MathematicaMathFun/wls/wtf-even-is-this.wls`, `projects/MathematicaMathFun/wls/symbol-mania.wls`, `projects/MathematicaMathFun/wls/ratata.wls`
- **Category / language-adjacent symbolic work**: `projects/MathematicaMathFun/wls/appy-thing.wls`, `projects/MathematicaMathFun/wls/complex-algebra.wls`, `projects/MathematicaMathFun/wls/connections.wls`, `projects/MathematicaMathFun/wls/grim.wls`

Interpretation: these files show an interest in symbolic expressiveness itself, not only in particular mathematical results.

### Data, economics, finance, and real-world entities

This is the most clearly applied branch. These files use Wolfram's data APIs to pull economic, administrative, market, and corporate data and then reshape or visualize it.

- **Macroeconomic data**: `projects/MathematicaMathFun/wls/gdp_by_1950_us_dollars.wls`, `projects/MathematicaMathFun/wls/more-inflation-computation.wls`, `projects/MathematicaMathFun/wls/just-some-fun.wls`, `projects/MathematicaMathFun/wls/beautiful-data.wls`
- **Sector and composition analysis**: `projects/MathematicaMathFun/sector_analysis.wls`, `projects/MathematicaMathFun/sector_percent_analysis.nb`, `projects/MathematicaMathFun/wls/pie-charts.wls`, `projects/MathematicaMathFun/pie-charts.wls`
- **Finance and statistical checks**: `projects/MathematicaMathFun/data_analysis.wls`, `projects/MathematicaMathFun/wls/stats.wls`, `projects/MathematicaMathFun/stats.wls`
- **Entity and company properties**: `projects/MathematicaMathFun/comp-prop-analysis.nb`

Interpretation: compared with the rest of the repo, this branch is more data-driven and less foundational; it uses Mathematica as a research notebook for economic and financial questions.

### Tooling, units, compilation, and miscellaneous technical experiments

Some files are not primarily about a mathematical theory but about Mathematica capabilities, units, compilation, or side utilities that support broader exploration.

- `projects/MathematicaMathFun/wls/compile-stuff.wls`
- `projects/MathematicaMathFun/wls/units-as-context.wls`
- `projects/MathematicaMathFun/wls/bottom-text.wls`
- `projects/MathematicaMathFun/wls/log-me-out.wls`

## Exhaustive grouped inventory

The following inventory is meant to account for the repo comprehensively, including exploratory files whose purpose is only partly explicit from the opening cells.

### A. Iteration and dynamics

- `projects/MathematicaMathFun/wls/fix_comp.wls`
- `projects/MathematicaMathFun/wls/flumoxed-and-blocked.wls`
- `projects/MathematicaMathFun/wls/found-it.wls`
- `projects/MathematicaMathFun/wls/gen-funcs.wls`
- `projects/MathematicaMathFun/wls/i-did-it.wls`
- `projects/MathematicaMathFun/wls/i-figured-it-out-i-was-right.wls`
- `projects/MathematicaMathFun/wls/i_fought_the_math_and_the_math_won.wls`
- `projects/MathematicaMathFun/wls/idk_what_im_doing.wls`
- `projects/MathematicaMathFun/wls/iter_as_complex_1.wls`
- `projects/MathematicaMathFun/wls/iter_as_matrix_rotation.wls`
- `projects/MathematicaMathFun/wls/iterate_algebra.wls`
- `projects/MathematicaMathFun/wls/iterate_my_func.wls`
- `projects/MathematicaMathFun/wls/iterated-rotation-success.wls`
- `projects/MathematicaMathFun/wls/iterated_arith_as_complex_num.wls`
- `projects/MathematicaMathFun/wls/iterated_calculus.wls`
- `projects/MathematicaMathFun/wls/iterated_coefficients.wls`
- `projects/MathematicaMathFun/wls/iteration_as_complex_algebra.wls`
- `projects/MathematicaMathFun/wls/iteration_as_graph.wls`
- `projects/MathematicaMathFun/wls/iteration_as_linear_trans.wls`
- `projects/MathematicaMathFun/wls/iteration_as_rotation.wls`
- `projects/MathematicaMathFun/wls/iteration_finished.wls`
- `projects/MathematicaMathFun/wls/iteration_rotation.wls`
- `projects/MathematicaMathFun/wls/real_iteration.wls`
- `projects/MathematicaMathFun/wls/series-iter.wls`

### B. Collatz, grammars, and parity logic

- `projects/MathematicaMathFun/wls/collatz-log-counting.wls`
- `projects/MathematicaMathFun/wls/collatz-op.wls`
- `projects/MathematicaMathFun/wls/collatz_grammar_almost_done.wls`
- `projects/MathematicaMathFun/wls/collatz_grammar_fix_this.wls`
- `projects/MathematicaMathFun/wls/collatz_grammar_methods_perfected.wls`
- `projects/MathematicaMathFun/wls/collatz_grammar_new_rules.wls`
- `projects/MathematicaMathFun/wls/collatz_log_stuff.wls`
- `projects/MathematicaMathFun/wls/collatz_template.wls`
- `projects/MathematicaMathFun/wls/discrete-alge.wls`
- `projects/MathematicaMathFun/wls/backtomath.wls`
- `projects/MathematicaMathFun/wls/enough_grammars_for_now.wls`
- `projects/MathematicaMathFun/wls/grammar_but_it_doesnt_end.wls`
- `projects/MathematicaMathFun/wls/grammar_deconstruction.wls`
- `projects/MathematicaMathFun/wls/grammar_fun.wls`
- `projects/MathematicaMathFun/wls/grammar_minimal.wls`
- `projects/MathematicaMathFun/wls/grammar_new_measure_metric.wls`
- `projects/MathematicaMathFun/wls/grammar_stuff.wls`
- `projects/MathematicaMathFun/wls/grammars_build_up.wls`
- `projects/MathematicaMathFun/wls/grammatical_stuff.wls`
- `projects/MathematicaMathFun/wls/i_am_a_grammarian_now.wls`
- `projects/MathematicaMathFun/wls/int-trans-logic.wls`
- `projects/MathematicaMathFun/wls/iteration_as_FSM.wls`
- `projects/MathematicaMathFun/wls/lang_id_at_limit.wls`
- `projects/MathematicaMathFun/wls/log-props.wls`
- `projects/MathematicaMathFun/wls/more_collatz_and_analysis.wls`
- `projects/MathematicaMathFun/wls/odd_even_odd_eq_proof.wls`
- `projects/MathematicaMathFun/wls/proofs_and_stuff.wls`
- `projects/MathematicaMathFun/wls/tick_tock.wls`
- `projects/MathematicaMathFun/wls/trees.wls`

### C. Complex analysis, transforms, and visualization

- `projects/MathematicaMathFun/complex-fun.wls`
- `projects/MathematicaMathFun/wls/I_am_satisfied_with_complex_stuff.wls`
- `projects/MathematicaMathFun/wls/a_complex_story.nb`
- `projects/MathematicaMathFun/wls/comp-ops.wls`
- `projects/MathematicaMathFun/wls/comp.wls`
- `projects/MathematicaMathFun/wls/complex-fun.wls`
- `projects/MathematicaMathFun/wls/complex-fun2.wls`
- `projects/MathematicaMathFun/wls/complex-iter-fun.wls`
- `projects/MathematicaMathFun/wls/complex_iterated.wls`
- `projects/MathematicaMathFun/wls/complex_nums.wls`
- `projects/MathematicaMathFun/wls/complex_nums_to_iter_unc.wls`
- `projects/MathematicaMathFun/wls/complex_plots.wls`
- `projects/MathematicaMathFun/wls/complex_visual.wls`
- `projects/MathematicaMathFun/wls/connections.wls`
- `projects/MathematicaMathFun/wls/decompose_into_len_and_rot.wls`
- `projects/MathematicaMathFun/wls/disc-ztr.wls`
- `projects/MathematicaMathFun/wls/func_as_complex_rot.wls`
- `projects/MathematicaMathFun/wls/i_finally_understand_complex_nums.wls`
- `projects/MathematicaMathFun/wls/laplace-again.wls`
- `projects/MathematicaMathFun/wls/laplace.wls`
- `projects/MathematicaMathFun/wls/log-zeta.wls`
- `projects/MathematicaMathFun/wls/mathy-stuff.wls`
- `projects/MathematicaMathFun/wls/maybe-fourier.wls`
- `projects/MathematicaMathFun/wls/oh-well.wls`
- `projects/MathematicaMathFun/wls/power-of-my-waves.wls`
- `projects/MathematicaMathFun/wls/signal-stugff.wls`
- `projects/MathematicaMathFun/wls/systems-op.wls`
- `projects/MathematicaMathFun/wls/what_am_i_even_doing.wls`
- `projects/MathematicaMathFun/wls/what_even_are_complex_nums.wls`
- `projects/MathematicaMathFun/wls/why-isnt-it-working.wls`

### D. Geometry, calculus, and continuous analysis

- `projects/MathematicaMathFun/calculus-of-var.wls`
- `projects/MathematicaMathFun/curvy-curves.wls`
- `projects/MathematicaMathFun/math_and_stuff.wls`
- `projects/MathematicaMathFun/wls/back_to_geo.wls`
- `projects/MathematicaMathFun/wls/calculus-of-var.wls`
- `projects/MathematicaMathFun/wls/contours-of-life.wls`
- `projects/MathematicaMathFun/wls/curvature_analysis.wls`
- `projects/MathematicaMathFun/wls/curvature_vs_dot_dir.wls`
- `projects/MathematicaMathFun/wls/curvy-curves.wls`
- `projects/MathematicaMathFun/wls/jordan-decomp.wls`
- `projects/MathematicaMathFun/wls/math.wls`
- `projects/MathematicaMathFun/wls/random_math_stuff_idk.wls`
- `projects/MathematicaMathFun/wls/spectral_theory.wls`
- `projects/MathematicaMathFun/wls/variation.wls`
- `projects/MathematicaMathFun/wls/x-exp.wls`

### E. Algebra, polynomials, symbolic mathematics, and discrete structure

- `projects/MathematicaMathFun/just_some_fun.wls`
- `projects/MathematicaMathFun/wls/alge-bruh.wls`
- `projects/MathematicaMathFun/wls/algebra_as_straight_edge_and_compass.wls`
- `projects/MathematicaMathFun/wls/appy-thing.wls`
- `projects/MathematicaMathFun/wls/complex-algebra.wls`
- `projects/MathematicaMathFun/wls/eveness_measure.wls`
- `projects/MathematicaMathFun/wls/evenness-measure2.wls`
- `projects/MathematicaMathFun/wls/grim.wls`
- `projects/MathematicaMathFun/wls/irrational_nums.wls`
- `projects/MathematicaMathFun/wls/just_some_fun.wls`
- `projects/MathematicaMathFun/wls/more-poly-stuff.wls`
- `projects/MathematicaMathFun/wls/poly-fun.wls`
- `projects/MathematicaMathFun/wls/ratata.wls`
- `projects/MathematicaMathFun/wls/studying-polys.wls`
- `projects/MathematicaMathFun/wls/symbol-mania.wls`
- `projects/MathematicaMathFun/wls/theres-something-about-polynomials.wls`
- `projects/MathematicaMathFun/wls/wtf-even-is-this.wls`

### F. Data, economics, finance, and entities

- `projects/MathematicaMathFun/comp-prop-analysis.nb`
- `projects/MathematicaMathFun/data_analysis.wls`
- `projects/MathematicaMathFun/pie-charts.wls`
- `projects/MathematicaMathFun/sector_analysis.wls`
- `projects/MathematicaMathFun/sector_percent_analysis.nb`
- `projects/MathematicaMathFun/stats.wls`
- `projects/MathematicaMathFun/wls/beautiful-data.wls`
- `projects/MathematicaMathFun/wls/gdp_by_1950_us_dollars.wls`
- `projects/MathematicaMathFun/wls/just-some-fun.wls`
- `projects/MathematicaMathFun/wls/more-inflation-computation.wls`
- `projects/MathematicaMathFun/wls/pie-charts.wls`
- `projects/MathematicaMathFun/wls/stats.wls`

### G. Tooling, units, utilities, and uncategorized scratch files

- `projects/MathematicaMathFun/wls/bottom-text.wls`
- `projects/MathematicaMathFun/wls/compile-stuff.wls`
- `projects/MathematicaMathFun/wls/log-me-out.wls`
- `projects/MathematicaMathFun/wls/units-as-context.wls`

## How to read this repo

- **Treat filenames as chronology**: many names read like progress markers, so related ideas often continue across several neighboring files.
- **Expect overlap**: the same mathematical question is often attacked from symbolic, geometric, and computational angles in parallel.
- **Expect incomplete branches**: some files are polished demonstrations, but many are checkpoints, failed attempts, or reduced testbeds.
- **Use the thematic notes as entry points**:
  - `notes/MathematicaMathFun/IterativeDynamics.md`
  - `notes/MathematicaMathFun/FormalLanguages.md`
  - `notes/MathematicaMathFun/AnalysisGeometry.md`
  - `notes/MathematicaMathFun/Economics.md`
  - `notes/MathematicaMathFun/Experimental.md`

## Summary

`MathematicaMathFun` is not one project; it is a long-running mathematical workspace. The most important intellectual through-lines are:

- iteration as a structure that should have its own algebra and geometry,
- Collatz and parity as symbolic-language phenomena,
- complex numbers as a unifying representation for dynamics,
- curvature and transforms as bridges between symbolic and visual reasoning,
- and Mathematica itself as the medium for rapidly testing conjectural mathematical ideas.

---

[Back to Main README](../README.md)
