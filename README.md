# EpiCats
Applied category theory applied to epidemiological models 

# Examples

## Petri nets
- [SIR model composed from infection and recovery submodels](https://github.com/epirecipes/EpiCats/pn_compose_sir/pn_compose_sir.md)
- [SIR model stratified by risk](https://github.com/epirecipes/EpiCats/pn_stratify_multigroup/pn_stratify_multigroup.md)

# Glossary of applied category theory applied to epidemiological models

| Term                                    | Definition                                                                                                                                    | Example in epidemiology                                                                                                                                                |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Category                                | Includes “objects” representing entities or states and “arrows” (morphisms) representing transitions or relationships between entities.       | Objects: different disease states of an individual (Susceptible, Infected, Recovered).                                                                                 |
| Morphism                                | A mapping, function or transformation from one object to another.                                                                             | The transformation of a person from a susceptible state to an infected state.                                                                                          |
| Domain                                  | The object from which the arrow or morphism originates.                                                                                       | For an arrow representing transmission, the domain would be the susceptible state.                                                                                     |
| Codomain                                | The object to which the arrow points.                                                                                                         | For an arrow representing transmission, the codomain would be the infected state.                                                                                      |
| Functor                                 | A mapping between categories that preserves the structure, by mapping objects to objects and arrows to arrows.                                | The effort of a vaccination program, where the functor maps the pre-vaccination states and transitions to the post-vaccination states and transitions.                 |
| Monad                                   | A structure that encapsulates side effects.                                                                                                   | Stochastic effects such as the randomness of disease transmission.                                                                                                     |
| Product                                 | The product of two objects in a category is a new object that captures the "essence" of both objects simultaneously.                          | The combination of age and vaccination classes to create ‘young/unvaccinated’ classes etc.                                                                             |
| Coproduct                               | Represents the "sum" or "choice" of two objects                                                                                               | A grouping of all vaccinated individuals across age classes.                                                                                                           |
| Pullback

(generalization

of product)  | Represents the most general object that maps to two given objects in a way that is compatible with a specified mapping between those objects. | Can represent interactions between different populations or compartments. Unlike a product, specific interactions can be selected, rather than all.                    |
| Pushout

(generalization

of coproduct) | Represents the most general object that two given objects map to, in a way that is compatible with a specified mapping between those objects. | Can be used to represent the fusion or aggregation of different disease states or populations. Unlike a coproduct, specific states can be chosen to be glued together. |
| Span                                    | A diagram consisting of two morphisms with a common domain                                                                                    | Leaving a susceptible state through infection or vaccination.                                                                                                          |
| Cospan                                  | A diagram consisting of two morphisms with a common codomain                                                                                  | Entering an immune state through either recovery or vaccination.                                                                                                       |
| Hom-set                                 | The set of all morphisms from one object to another in a category.                                                                            | All possible transitions between a pair of states; in an SIR model, there would be a hom-set between S and I composed of the morphism representing transmission.       |
