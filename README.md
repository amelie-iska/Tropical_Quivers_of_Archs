[![Paper](https://img.shields.io/badge/PDF-Download%20Paper-blue)](./tropical_quiver_research_program.pdf) [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Blog%20Post-ffcc4d)]()

This paper develops a ground-up research program for *composable learned operators* in which every internal module is viewed through a *tropical lens* and every architecture is represented as a *decorated quiver of embedding spaces*.
The organizing principle is boundary-aware:
discrete token spaces appear only at *source encoder* vertices and *sink decoder* vertices, while all intermediate computation lives in differentiable embedding spaces connected by general adapters, projections, cross-attention interfaces, residual merges, and neural-operator couplings.
This perspective is designed to cover standard transformers and their descendants---including ViT, DiT, SiT, multimodal fusion stacks, diffusion/flow transformers, state-space hybrids, and scientific foundation-model pipelines---while also extending to non-transformer modules.

The mathematical thesis is that modular deep systems should be studied as *quivers of tropicalized operators*.
Piecewise-linear modules induce exact tropical rational maps and activation fans; transformer blocks become compositions of tropicalizable linear projections, piecewise-linear feed-forward layers, and tropical or locally tropicalized attention kernels; smooth modules admit local tropical charts on compact energy shells.
Composing such modules yields *composed tropical spaces*: polyhedral atlases, tropical varieties, and scheme-like glued cell complexes attached to paths and cycles of the quiver.
This makes the geometry of composability explicit rather than hidden inside a global linear surrogate.

For cyclic quivers we develop a joint *tropical-dynamical-ergodic* viewpoint.
Activation itineraries define symbolic dynamics on cell complexes; max-plus and subadditive cocycles quantify long-run growth; invariant measures describe occupancy of activation fans; and Navier--Stokes-inspired "thought-fluid" regularization constrains continuous Graph-of-Thought trajectories in embedding space.
The reward structure is integrated with *hybrid continuous-discrete GFlowNets*: graph construction trajectories and continuous reasoning trajectories are both sampled with probability proportional to multiobjective rewards that favor high-quality solutions subject to explicit resource constraints.
We also show how recent activation-steering ideas, exemplified by the ``Assistant Axis,'' can be lifted to quiver-local tropical steering atlases that regulate both instantaneous embedding updates and long-run ergodic occupancy of activation regions.

The manuscript emphasizes formal definitions, rigorous propositions, implementation-oriented algorithms, and realistic examples.
These include continuous GoT reasoning GFlowNets, multimodal source/sink compositions linking NatureLM-style cross-domain sequence reasoning to MDGen-style SiT generative dynamics, and multi-model therapeutic design cycles that couple generators, evaluators, structure predictors, cell-state models, and phenotype or variant predictors through adapter-mediated embedding spaces.
The result is a tropical, quiver-theoretic, ergodic framework for architecture design and search that is intended to be both mathematically serious and practically actionable.
