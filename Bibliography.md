# Resources for the NbE reading group

## Read in the reading group

- [Streicher's short note](https://www2.mathematik.tu-darmstadt.de/~streicher/snbe.pdf) and the longer [Categorical reconstruction of a reduction free normalization proof](https://www.tcs.ifi.lmu.de/mitarbeiter/martin-hofmann/pdfs/categoricalreconstruction.pdf) (1995, Altenkirch Hoffmann Streicher): early categorical approach, however it does not use proper gluing, only an ad-hoc twisted gluing construction.
- [Andreas Abel's Habilitation Thesis](https://www.cse.chalmers.se/~abela/publications.html#habil): non-categorical approach, using untyped syntax and "traditional" logical relation; scales to depedent type systems rather easily, although the argument becomes somewhat more complicated, the NbE algorithm itself is mostly unchanged.
- [Semantic analysis of normalisation by evaluation for typed lambda calculus](https://www.cambridge.org/core/journals/mathematical-structures-in-computer-science/article/semantic-analysis-of-normalisation-by-evaluation-for-typed-lambda-calculus/E3727362B3E059149680CC3482FFDCFC) (Fiore, 2002, new version in 2022): more mature categorical approach, using vanilla gluing instead of an ad-hoc construction; based on intrinsically well-typed syntax/initial CCC.

## More things that are probably interesting to look at

### Other "core NbE" papers

- [Normalization and the Yoneda Embedding](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/52CC6B0D0961F134ABF28BF6A824D45B/S0960129597002508a.pdf/normalization-and-the-yoneda-embedding.pdf): categorical approach, but based on P-category theory (PER-enriched).
- [Canonicity and normalisation for Dependent Type Theory](https://arxiv.org/abs/1810.09367): typical dense but efficient Coquand paper.

### Implementations

- [Implementing a modal dependent type theory](https://dl.acm.org/doi/abs/10.1145/3341711), and its [implementation](https://github.com/jozefg/blott): the implementation part is quite close to Abel's approach, but the proofs are more categorical; probably a good place to look at these ideas applied in a "modern" implementation.
- Other related implementations (in ML) of NbE for dependent types: [vanilla MLTT](https://github.com/jozefg/nbe-for-mltt), and [a multi-modal dependent type theory](https://github.com/logsem/mitten_preorder).
- [Full Reduction at Full Throttle](https://link.springer.com/chapter/10.1007/978-3-642-25379-9_26): implementation of Coq's `native_compute`, an NbE evaluator using OCaml's abstract machine.

### Formalizations

- [A Machine-Checked Correctness Proof of Normalization by Evaluation for Simply Typed Lambda Calculus](https://andraskovacs.github.io/pdfs/mscthesis.pdf) (András Kovács master thesis).
- [A Coq formalization of normalization by evaluation for Martin-Löf type theory](https://dl.acm.org/doi/abs/10.1145/3167091): formalization, in Coq, of NbE for a dependently typed system (but without large elimination), following Abel.

### Applications and relations to other fields

- [A functional correspondence between evaluators and abstract machines](https://dl.acm.org/doi/abs/10.1145/888251.888254): relation between the NbE and abstract machine approaches.
- [Coherence for bicategorical cartesian closed structure](https://www.cambridge.org/core/journals/mathematical-structures-in-computer-science/article/coherence-for-bicategorical-cartesian-closed-structure/9AF32A2CDBDD01A5FB01D9D6DDCD80F0): NbE technique to show strictification/coherence properties.

### Synthetic Tait Computability

- Sterling's [lecture notes](https://www.jonmsterling.com/papers/sterling-2022-naive.pdf) for the Types WG6 in April 2022
- His [dissertation overview](https://www.jonmsterling.com/forest/trees/jms-000q/)
- And of course, his [PhD](https://www.jonmsterling.com/bibliography.html#dissertations)
- [Synthetic Tait Computability the Hard Way](https://arxiv.org/abs/2310.02051) seems like a "pedestrian" approach to the technique?

## More papers that are probably less relevant nowadays

- [Notes on sconing and relators](https://link.springer.com/chapter/10.1007/3-540-56992-8_21) (early usage of glueing?)
- [Type-directed partial evaluation](https://dl.acm.org/doi/abs/10.1145/237721.237784) (the og paper)
