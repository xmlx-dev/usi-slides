[![View Slides][slides-badge]](https://usi.xmlx.dev)
[![GitHub Release](https://img.shields.io/github/v/release/xmlx-dev/usi-slides?display_name=tag&logo=github)](https://github.com/xmlx-dev/usi-slides/releases/latest)  
[![Slides Licence](https://img.shields.io/badge/slides%20licence-CC%20BY--NC--SA%204.0-lightgrey)](LICENCE)
[![Code Licence](https://img.shields.io/badge/code%20licence-MIT-lightgrey)](LICENCE-code)  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7646970.svg)](https://doi.org/10.5281/zenodo.7646970)
[![Cite BibTeX](https://img.shields.io/badge/cite-bibtex-yellow.svg)](https://usi.xmlx.dev/slides/index.html#citing-the-slides)

#  Machine Learning Explainability
## Exploring Automated Decision-Making Through Transparent Modelling and Peeking Inside Black Boxes

---

## Course Summary

Machine learning models require care, attention and a fair amount of tuning to
offer accurate, consistent and robust predictive modelling of data.
Why should their transparency and explainability be any different?
While it is possible to easily generate explanatory insights with methods that
are post-hoc and model-agnostic -- LIME and SHAP, for example -- these can be
misleading when output by generic tools and viewed out of (technical or
domain) context.
Explanations should not be taken at their face value;
instead their understanding ought to come from interpreting explanatory
insights in view of the implicit caveats and limitations under which they
were generated.
After all, explainability algorithms are complex entities often built from
multiple components that are subject to parameterisation choices and
operational assumptions, all of which must be accounted for and configured
to yield a truthful and useful explainer.
Additionally, since any particular method may only provide partial information
about the functioning of a predictive model, embracing diverse insights and
appreciating their complementarity -- as well as disagreements -- can further
enhance understanding of an algorithmic decision-making process.

This course takes an adversarial perspective on artificial intelligence
explainability and machine learning interpretability.
Instead of reviewing popular approaches used to these ends, it breaks them
up into core functional blocks, studies the role and configuration thereof,
and reassembles them to create bespoke, well-understood explainers suitable
for the problem at hand.
The course focuses predominantly on tabular data, with some excursions into
image and text explainability whenever a method is agnostic of the data type.
The tuition is complemented by a series of hands-on materials for self-study,
which allow you to experiment with these techniques and appreciate their
inherent complexity, capabilities and limitations.
The assignment, on the other hand, requires you to develop a tailor-made
explainability suite for a data set and predictive model of your choice,
or alternatively analyse an explainability algorithm to identify
its core algorithmic building blocks and explore how they affect the resulting
explanation.
(Note that there is a scope for a bespoke project if you have a well-defined
idea in mind.)

## Curriculum

(*Reveal the topics covered in each theme by clicking the triangle button*.)

<details>
<summary><u>
Introduction to explainability
</u></summary>

* History of explainability
* Types of explanations
* Taxonomy and classification of explainability approaches
* A human-centred perspective
* Ante-hoc vs. post-hoc discussion
* Multi-class explainability
* Defining explainability
* Evaluation of explainability techniques

</details>

<details>
<summary><u>
A brief overview of data explainability
</u></summary>

* Data as an (implicit) model
* Data summarisation and description
* Dimensionality reduction
* Exemplars, prototypes and criticisms

</details>

<details>
<summary><u>
Transparent modelling
</u></summary>

* The ante-hoc vs. post-hoc distinction in view of information lineage
  (i.e., endogenous and exogenous sources of information that form
  the explanations)
* Rule lists and sets
* Linear models (and generalised additive models)
* Decision trees
* $k$-nearest neighbours and $k$-means

</details>

<details>
<summary><u>
Feature importance
</u></summary>

* Permutation Importance
* Feature Interaction

</details>

<details>
<summary><u>
Feature influence
</u></summary>

* Individual Conditional Expectation
* Partial Dependence
* LIME
* SHAP
* Accumulated Local Effects

</details>

<details>
<summary><u>
Exemplars
</u></summary>

* Exemplar explanations
* Counterfactuals
* Prototypes and criticisms

</details>

<details>
<summary><u>
Rules
</u></summary>

* Scoped rules
* ANCHOR
* RuleFit

</details>

<details>
<summary><u>
Meta-explainers
</u></summary>

* Local, cohort and global surrogates

</details>

## Projects

Two types of a (possibly group-based) assignment are envisaged.
(*However, if you have a well-defined project in mind, you may be allowed to
pursue it -- in this case talk to the course instructors.*)

1. *Develop a bespoke explainability suite for a predictive model of your
   choice.*
   If you are working on a machine learning project that could benefit from
   explainability, this project presents an opportunity to use the course as
   a platform to this end.
   Alternatively, you can explore explainability of a pre-existing model
   available to download or accessible through a web API.

2. *Choose an explainability method and identify its core algorithmic building
   blocks to explore how they affect the final explanations.*
   You are free to explore explainability of inherently transparent models,
   develop model-specific approaches for an AI or ML technique that interests
   you, or pursue a model-agnostic technique.

> For students who would like to learn more about explainable artificial
> intelligence and interpretable machine learning but cannot dedicate the
> time necessary to complete the assignment due to other commitments,
> there is a possibility of a lightweight project.
> In this case you can choose an explainability method and articulate its
> assumptions as well as any discrepancies from its (most popular)
> implementation -- possibly based on some of the (interactive) course
> materials -- as long as you present your findings at the end of the course.

The projects will be culminated in presentations and/or demos delivered in
front of the entire cohort.
The project delivery should focus on reproducibility of the results and
quality of the investigation into explainability aspects of the chosen system,
therefore *the journey is more important than the outcome*.
Under this purview, all of the assumptions and choices -- theoretical,
algorithmic, implementation and otherwise -- should be made explicit and
justified.
You are *strongly encouraged* to prepare and present your findings via one of
the dashboarding or interactive reporting/presentation tools
(see the list of options [included below](#useful-resources)),
however this aspect of the project is *optional*.

---

**Examples**  
(*See the description of each example project by clicking
the triangle button*.)

<details>

<summary><u>
Identify the sources of explanation (dis)agreements for a given predictive
modelling task
</u></summary>

> For a given data set -- e.g., MNIST -- one can train a collection of
> transparent and black-box models;
> for example, linear classifiers, decision trees, random forests,
> support vector machines (with different kernels), logistic regressions,
> perceptrons, neural networks.
> If the chosen data set lends itself to natural interpretability, i.e.,
> instances (and their features) are understandable to humans, these models
> can be explained with an array of suitable techniques and their
> explanations compared and contrasted.
> Such experiments can help to better understand capabilities and limitations
> of individual explainability techniques, especially when their composition,
> configuration and parameterisation is considered.
> This can lead to practical guidelines on using these explainers and
> interpreting their results.

</details>

<details>

<summary><u>
New composition of an existing explainability technique
</u></summary>

> When functionally independent building blocks of an explainability approach
> can be isolated, we can tweak or replace them to compose a more robust and
> accountable technique.
> Similarly, a well-known explainer can be expanded with a new explanatory
> artefact or modality, e.g., a counterfactual statement instead of feature
> importance/influence.
> Additionally, comparing the explanations output by the default and
> bespoke methods can help to uncover discrepancies that may be abused in
> order to generate misleading explanatory insights;
> for example, explainees can be deceived by presenting them with an
> explanation based on a specifically crafted sample of data (used with
> post-hoc methods).

</details>

<details>

<summary><u>
New explainability technique from existing building blocks
</u></summary>

> Instead of improving a pre-existing explainability technique, algorithmic
> components from across the explainability spectrum can become an inspiration
> to build an entirely new explainer or explainability pipeline.

</details>

<details>

<summary><u>
Explore the behaviour of a pre-existing model with explainability techniques
</u></summary>

> Given the success of deep learning in predictive modelling, opaque systems
> based on ML algorithms often end up in production.
> While it may be difficult to identify any of their undesirable properties
> from the outset, these are often discovered (and corrected) throughout the
> lifespan of such systems.
> In this space, explainability techniques may help to uncover these
> characteristic and pinpoint their sources, potentially leading to
> observations that reveal biases or aid in scientific discoveries.
> Either of these applications can have significant social impact and benefit,
> leading to these models being corrected or decommissioned.
> Sometimes, however, their idiosyncrasies can be observed, but their origin
> remains unaccounted for.
> For example, consider the case of machine learning models dealing with
> chest X-rays, which additionally can detect the race of the patients --
> something that doctors are incapable of discerning
> (see [here][xray-wired] and [here][xray-dataconomy] for more details).
> While the reason for this behaviour remains a mystery, a thorough
> investigation of this, and similar, models with an array of well-understood
> (post-hoc) explainability techniques may be able to offer important clues.

</details>

## Schedule

The course will span *two weeks*, offering the following tuition each day
(*ten days total*):

- 1-hour lecture;
- 1-hour supervised lab session (system design and coding); and
- half-an-hour open office (general questions and project discussions).

The lectures will roughly follow the curriculum outlined above.
The envisaged self-study time is around 20 hours, which largely involves
completing a project of choice (possibly in small groups).

## Learning Objectives

**General**

- Understand the landscape of AI and ML explainability techniques.
- Identify explainability needs of data-driven machine learning systems.
- Recognise the capabilities and limitations of explainability approaches,
  both in general and in view of specific use cases.
- :star: Apply these skills to real-life AI and ML problems.
- :star: Communicate explainability findings through interactive reports and
  dashboards.

**Specific to explainability approaches**

- Identify self-contained algorithmic components of explainers and
  understand their functions.
- Connect these building blocks to the explainability requirements unique to
  the investigated predictive system.
- Select appropriate algorithmic components and tune them to the problem at
  hand.
- Evaluate these building blocks (in this specific context) independently and
  when joined together to form the final explainer.
- Interpret the resulting explanations in view of the uncovered properties and
  limitations of the bespoke explainability algorithm.

## Prerequisites

- Python programming.
- Familiarity with basic mathematical concepts (relevant to machine learning).
- Knowledge of machine learning techniques for tabular data.
- :star: Prior experience with machine learning approaches for images and text
  (e.g., deep learning) or other forms of data modelling (e.g., time series
  forecasting, reinforcement learning) if you decide to pursue a project in
  this direction.

## Useful Resources

- :book: Books

    * [Survey of machine learning interpretability][iml]
      in form of an online book
    * Overview of [explanatory model analysis][ema] published as
      an online book

- :memo: Papers

    * General introduction to [interpretability][beholder]
    * Introduction to [human-centred explainability][miller]
    * Critique of [post-hoc explainability][rudin]
    * Survey of [interpretability techniques][guidotti]
    * [Taxonomy of explainability approaches][taxonomy]

- :minidisc: Explainability software

    * LIME ([Python][lime-py], [R][lime-r])
    * SHAP ([Python][shap-py], [R][shap-r])
    * Microsoft's [Interpret][interpret]
    * Oracle's [Skater][skater]
    * IBM's [Explainability 360][ex360]
    * [FAT Forensics][fatf]

- :minidisc: Interactive dashboarding software

    * [Streamlit][streamlit]
    * [Plotly Dash][dash]
    * Shiny for [Python][shiny-py] and [R][shiny-r]
    * [Quarto][quarto]

## Instructor

**Kacper Sokol**
(*<Kacper.Sokol@rmit.edu.au>*; *<K.Sokol@bristol.ac.uk>*)

> Kacper is a Research Fellow at the ARC Centre of Excellence for Automated
> Decision-Making and Society (ADM+S), affiliated with the School of Computing
> Technologies at RMIT University, Australia, and an Honorary Research Fellow
> at the Intelligent Systems Laboratory, University of Bristol, United Kingdom.
>
> His main research focus is transparency -- interpretability and
> explainability -- of data-driven predictive systems based on artificial
> intelligence and machine learning algorithms.
> In particular, he has done work on enhancing transparency of predictive
> models with *feasible and actionable counterfactual explanations* and
> *robust modular surrogate explainers*.
> He has also introduced *Explainability Fact Sheets* -- a comprehensive
> taxonomy of AI and ML explainers -- and prototyped
> *dialogue-driven interactive explainability systems*.
>
> Kacper is the designer and lead developer of *FAT Forensics* -- an open
> source fairness, accountability and transparency Python toolkit.
> Additionally, he is the main author of a collection of online interactive
> *training materials about machine learning explainability*, created in
> collaboration with the Alan Turing Institute -- the UK's national institute
> for data science and artificial intelligence.
>
> Kacper holds a Master's degree in Mathematics and Computer Science, and a
> doctorate in Computer Science from the University of Bristol, United Kingdom.
> Prior to joining ADM+S he has held numerous research posts at the
> University of Bristol, working with projects such as REFrAMe, SPHERE and
> TAILOR -- European Union's AI Research Excellence Centre.
> Additionally, he was a visiting researcher at the
> University of Tartu (Estonia);
> Simons Institute for the Theory of Computing, UC Berkeley (California, USA);
> and USI -- Università della Svizzera italiana (Lugano, Switzerland).
> In his research, Kacper collaborated with numerous industry partners,
> such as THALES, and provided consulting services on explainable artificial
> intelligence and transparent machine learning.

---

## Citing the Slides

If you happen to use these slides, please cite them as follows.

```bibtex
@misc{sokol2023explainable,
  author={Sokol, Kacper},
  title={{eXplainable} {Machine} {Learning} -- {USI} {Course}},
  howpublished={\url{https://usi.xmlx.dev/}},
  doi={10.5281/zenodo.7646970},
  year={2023}
}
```

## Acknowledgement

The creation of these educational materials was supported by
the ARC Centre of Excellence for Automated Decision-Making and Society
(project number CE200100005), and funded in part by the Australian Government
through the Australian Research Council.

<!-- articles -->
[xray-wired]: https://www.wired.com/story/these-algorithms-look-x-rays-detect-your-race/
[xray-dataconomy]: https://dataconomy.com/2022/06/ai-can-tell-peoples-race-from-x-rays/
<!-- books -->
[iml]: https://christophm.github.io/interpretable-ml-book/
[ema]: https://ema.drwhy.ai/
[xml]: #usefulresources
<!-- papers -->
[beholder]: https://arxiv.org/abs/2112.14466
[taxonomy]: https://arxiv.org/abs/1912.05100
[miller]: https://arxiv.org/abs/1706.07269
[rudin]: https://www.nature.com/articles/s42256-019-0048-x
[guidotti]: https://arxiv.org/abs/1802.01933
<!-- software -->
[lime-py]: https://lime-ml.readthedocs.io/en/latest/
[lime-r]: https://cran.r-project.org/web/packages/lime/vignettes/Understanding_lime.html
[shap-py]: https://shap.readthedocs.io/en/latest/
[shap-r]: https://cran.r-project.org/web/packages/shapr/vignettes/understanding_shapr.html
[interpret]: https://interpret.ml/docs/getting-started
[skater]: https://oracle.github.io/Skater/overview.html
[ex360]: https://aix360.readthedocs.io/en/latest/
[fatf]: https://fat-forensics.org/
[streamlit]: https://streamlit.io/
[dash]: https://dash.plotly.com/
[shiny-py]: https://shiny.rstudio.com/py/
[shiny-r]: https://shiny.rstudio.com/
[quarto]: https://quarto.org/

[slides-badge]: https://img.shields.io/badge/view-slides-blue.svg?logo=data:image/png;base64,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
