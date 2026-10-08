# Two triangulations sharing only five edges

For each n from 9 to 17, a set of n points in general position with two triangulations whose only common edges are the five edges of the convex hull. Together with a lower bound of 5 and an insertion step that passes from n to n + 1, this gives f(n) = 5 for every n >= 9, where f(n) is the least number of edges two triangulations of the same n points can share.

Context: MathOverflow question [Minimum number of common edges of triangulations](https://mathoverflow.net/q/454425) ([answer](https://mathoverflow.net/a/515648)).

## Contents

- `certificates/nNN.json`: the points (`points`, integer coordinates) and the edges of the two triangulations (`A` and `B`, as pairs of point indices). Each triangulation has 3n - 8 edges, and the two share exactly the five hull edges.
- `figures/nNN.png`: both triangulations drawn for each n; `figures/insertion_step.png`: the step from n to n + 1.
- `paper/`: a draft write-up of 30 September 2026. It has not been refereed, and a revised version is in preparation.

Claude Opus 5.5 and Claude Fable 5.1 (Anthropic) were used to search for examples, write and run the verification code, develop and check the proofs, and draft the paper. The author has checked the argument.

## Licence

Certificates, figures and paper are released under [CC BY 4.0](LICENSE).
