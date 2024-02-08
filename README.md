# Introduction #

This notebook showcases the application of a linear logistic decoder to neural activity data recorded in freely behaving mice during competition against other mice. The model is used to decode:

1. Whether the animal is winning or losing
2. Whether the animal is in a competitive context, in other words, whether the mouse is competing or alone in its home environment
3. Individual bouts of competitive behaviors (e.g., pushing of the opponent, resisting, or retreating)
The tube test

Activity is recorded during the tube test, a test of dominance relationships in mice, where two animals are inserted into a tube that is too narrow for turning, leading to one of the animals to push the other one out of the tube and winning the test. Annotated behaviours during this test are pushing, retreating, resisting the push of the opponent mouse.

![alt text](https://github.com/neven-x/Competitive-behaviour-encoding/blob/main/Tube%20test.png)

The activity was recorded from two brain areas in the mouse hypothalamus, the medial preoptic area (MPOA) and the ventromedial hypothalamus (VMH) using an implanted lens, which allows imaging of neuronal activity in vivo in cells expressing an optical indicator of cellular calcium concentration.

Example recording visualisation - red bars indicate tube tests, blue bars indicate first contact between the two mice

![alt text](https://github.com/neven-x/Competitive-behaviour-encoding/blob/main/Example%20TT%20recording.png)

This notebook explores which variables related to competition in this test can be decoded from hypothalamic population activity. The first two variables can be decoded significantly better compared to a model trained on shuffled labels, but not the third variable.

# Disclaimer #
This analysis is based on unpublished raw data which is not included in the repo.
