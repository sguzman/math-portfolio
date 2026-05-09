# Collatz Junk

`projects/collatz-junk` is a focused Mathematica repository for studying the Collatz conjecture from several exploratory angles. Compared with `MathematicaMathFun`, which treats Collatz as one thread among many, this repo is narrower and more concentrated: nearly every file attacks the parity-switching dynamics of Collatz directly.

## Scope

- **Primary medium**: Wolfram Language scripts with several Mathematica notebooks.
- **Directory structure**: almost all research lives under `projects/collatz-junk/notes`.
- **Main object of study**: the standard Collatz map, its parity sequence, its recursive behavior, and alternative analytic or symbolic encodings of the same process.

## Main research directions

### Parity sequences as symbolic language

A major line of attack is to convert Collatz trajectories into odd/even symbol strings and then analyze those strings as formal objects.

- Core sequence builders appear in:
  - `projects/collatz-junk/notes/collatz.wls`
  - `projects/collatz-junk/notes/collatz-seq.wls`
  - `projects/collatz-junk/notes/collatz-full-seq.wls`
  - `projects/collatz-junk/notes/collatz_template.wls`
- The parity map `odd -> o`, `even -> e` is used repeatedly to turn numerical trajectories into word-like objects.
- The main goal is not only to count odd and even events, but to identify recurring local patterns and compress them into reusable “grammar rules.”

This is one of the clearest places in the portfolio where Collatz is treated as a language-generation problem rather than only an arithmetic recurrence.

### Grammar and rewrite-system analysis

Several files explicitly build sequence-replacement systems over parity words:

- `projects/collatz-junk/notes/collatz-grammar.wls`
- `projects/collatz-junk/notes/collatz_e_o_complete_grammar.wls`
- `projects/collatz-junk/notes/collatz_grammar_analysis_via_vector_space.wls`
- `projects/collatz-junk/notes/collatz_most_explanative_grammar_rules.wls`
- `projects/collatz-junk/notes/collatz_ratio_measure.wls`
- `projects/collatz-junk/notes/a_collatz_cached.wls`

The repeated pattern is:

- compute a long Collatz trajectory,
- map it to an odd/even sequence,
- search for frequent subsequences,
- compress those subsequences into replacement symbols,
- and then study the reduced word or its statistics.

This is a meaningful research move. It suggests that the arithmetic difficulty of Collatz may be re-expressed as a combinatorial or grammatical regularity problem.

### Real-analytic or continuous parity switching

Another strong theme is replacing the discrete odd/even branch with a real-analytic selector using trigonometric parity detectors such as:

- `tick[n] = (1 + Cos[π n]) / 2`
- `tock[n] = 1 - tick[n]`

This appears in:

- `projects/collatz-junk/notes/collatz-full-seq.wls`
- `projects/collatz-junk/notes/collatz_alternative_to_trig_clock.wls`
- `projects/collatz-junk/notes/collatz_but_i_give_up_for_now.wls`
- `projects/collatz-junk/notes/collatz_but_its_unsolvable.wls`
- `projects/collatz-junk/notes/collatz_i_think.wls`
- `projects/collatz-junk/notes/collatz_the_world_is_not_enough.nb`
- `projects/collatz-junk/notes/collatz_why_are_we_here.wls`
- `projects/collatz-junk/notes/real-collatz.wls`

The underlying idea is to build a continuous or complex-analytic analogue of the Collatz rule by encoding parity as a smooth oscillatory function. That matters because it opens the door to:

- complex plots,
- iterative analysis over reals or complexes,
- transform-based study,
- and possible connections to operator or dynamical-systems techniques.

This is one of the most distinctive ideas in the repo.

### Pattern mining and local statistical structure

Some files study repeated subsequences, ratio-like measures, or local parity frequencies rather than global convergence proofs.

- `projects/collatz-junk/notes/collatz_ratio_measure.wls`
- `projects/collatz-junk/notes/collatz_running_out_of_ideas.wls`
- `projects/collatz-junk/notes/collatz_also_patterns.nb`
- `projects/collatz-junk/notes/collatz_in_the_jungle.nb`

The emphasis here is to detect structure in:

- tallies of parity words,
- partitions of trajectories into local windows,
- weighted subsequence frequency,
- and measures derived from long runs of Collatz data.

This line of attack assumes that if Collatz has hidden regularity, it may show up first as repeated local motifs before it appears as a full theorem.

### Recursive evaluation and caching

There is also a practical computational thread: many scripts are concerned with memoization, recursion limits, and efficient generation of long Collatz sequences.

- `projects/collatz-junk/notes/collatz_cached.wls`
- `projects/collatz-junk/notes/collatz_with_more_caching.wls`
- `projects/collatz-junk/notes/a_collatz_cached.wls`
- `projects/collatz-junk/notes/testing-caching.wls`
- `projects/collatz-junk/notes/recursion-limimt.wls`

This part of the repo is not secondary. For this style of research, computational tractability matters because:

- long trajectories are needed to mine patterns,
- memoization changes what experiments are affordable,
- and recursion behavior is itself part of how Collatz is being operationalized in code.

### Graph and structural visualization

Some notebooks explore graph-style views of the odd/even dynamics or related structural presentations:

- `projects/collatz-junk/notes/collatz_also_patterns.nb`
- `projects/collatz-junk/notes/collatz_in_the_jungle.nb`

These are less polished than the more formal grammar files, but they fit the wider portfolio habit of turning symbolic or iterative structure into visual objects.

## File groups

### Minimal core definitions

- `projects/collatz-junk/notes/collatz.wls`
- `projects/collatz-junk/notes/collatz-seq.wls`
- `projects/collatz-junk/notes/collatz-full-seq.wls`
- `projects/collatz-junk/notes/collatz_template.wls`

These define the baseline recursive map and build sequences for later experiments.

### Grammar-centric files

- `projects/collatz-junk/notes/collatz-grammar.wls`
- `projects/collatz-junk/notes/collatz_e_o_complete_grammar.wls`
- `projects/collatz-junk/notes/collatz_grammar_analysis_via_vector_space.wls`
- `projects/collatz-junk/notes/collatz_most_explanative_grammar_rules.wls`
- `projects/collatz-junk/notes/collatz_ratio_measure.wls`

These are the strongest evidence that the repo is trying to compress Collatz into a symbolic rewrite system.

### Real/complex analytic extensions

- `projects/collatz-junk/notes/collatz_alternative_to_trig_clock.wls`
- `projects/collatz-junk/notes/collatz_i_think.wls`
- `projects/collatz-junk/notes/collatz_the_world_is_not_enough.nb`
- `projects/collatz-junk/notes/collatz_why_are_we_here.wls`
- `projects/collatz-junk/notes/real-collatz.wls`

These files extend the discrete rule into real-analytic or complex-plot-friendly form.

### Experimental notebooks and dead ends

- `projects/collatz-junk/notes/collatz_but_i_give_up_for_now.wls`
- `projects/collatz-junk/notes/collatz_but_its_unsolvable.wls`
- `projects/collatz-junk/notes/collatz_but_then_i_got_sidetracked_by_12.1_features.nb`
- `projects/collatz-junk/notes/collatz_in_the_jungle.nb`
- `projects/collatz-junk/notes/collatz_running_out_of_ideas.wls`

The filenames are candid, but the content is useful: they document the failed branches, side explorations, and temporary hypotheses that accompanied the main research direction.

## How this repo fits the rest of the portfolio

`collatz-junk` sits between several other portfolio areas:

- It overlaps with `notes/MathematicaMathFun.md` on Collatz, grammars, and iterative dynamics.
- It overlaps with `notes/articles/math.md` on operator-theoretic Collatz, parity formalization, and continuous analogues of discrete rules.
- It overlaps with `notes/MathWhiteBoard.md` in the tendency to turn symbolic dynamics into structural or visual objects.

The difference is focus: this repo is a dedicated Collatz workshop.

## Summary

The key research contribution of `projects/collatz-junk` is not a single theorem. It is the concentration of multiple lines of attack on the same problem:

- Collatz as a parity language,
- Collatz as a rewrite grammar,
- Collatz as a real-analytic branch-switching system,
- Collatz as a pattern-mining problem over long trajectories,
- and Collatz as a computational object whose structure can be exposed by caching, transforms, and visual reformulation.

That makes it an important addition to this portfolio, especially because it sharpens one of the most persistent themes across the broader body of work: iteration deserves richer mathematics than repeated substitution alone.

---

[Back to Main README](../README.md)
