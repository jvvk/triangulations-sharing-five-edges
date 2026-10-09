# Two triangulations sharing only five edges

<!-- visual:start -->
<p align="center"><img src="https://raw.githubusercontent.com/jvvk/jvvk/c7403d6bbbc7106e1780d8c34833854afcb0116f/assets/triangulations.svg" width="760" alt="triangulations-sharing-five-edges"></p>

<p align="center"><b>From nine points on, two triangulations can share nothing but the five outline edges, answering Rote.</b></p>

<p align="center"><sub><a href="https://github.com/jvvk/mathematics/tree/main/two-triangulations-hull">the paper, with its checks</a> · <a href="https://github.com/jvvk/mathematics">all results</a></sub></p>
<!-- visual:end -->

For each n from 9 to 17, a set of n points in general position with two triangulations whose only common edges are the five edges of the convex hull. Together with a lower bound of 5 and an insertion step that passes from n to n + 1, this gives f(n) = 5 for every n >= 9, where f(n) is the least number of edges two triangulations of the same n points can share.

Context: MathOverflow question [Minimum number of common edges of triangulations](https://mathoverflow.net/q/454425) ([answer](https://mathoverflow.net/a/515648)).

## Contents

- `certificates/nNN.json`: the points (`points`, integer coordinates) and the edges of the two triangulations (`A` and `B`, as pairs of point indices). Each triangulation has 3n - 8 edges, and the two share exactly the five hull edges.
- `figures/nNN.png`: both triangulations drawn for each n; `figures/insertion_step.png`: the step from n to n + 1.
- `paper/`: the write-up as it stood on 30 September 2026, when the answer was posted. It has not been refereed. The current version, which also settles every hull size, is in [jvvk/mathematics/two-triangulations-hull](https://github.com/jvvk/mathematics/tree/main/two-triangulations-hull), with the exact checker and the Lean formalisation.

Claude Opus 5.5 and Claude Fable 5.1 (Anthropic) were used to search for examples, write and run the verification code, develop and check the proofs, and draft the paper. The author has checked the argument.

## Licence

Certificates, figures and paper are released under [CC BY 4.0](LICENSE).
