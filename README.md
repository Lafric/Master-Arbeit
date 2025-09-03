# Table presenting the common points between different reproducibility checklists standards (recommandations for papers): 

- Paper On Reproducible AI : [https://www.researchgate.net/publication/327942340_On_Reproducible_AI_Towards_Reproducible_Research_Open_Science_and_Digital_Scholarship_in_AI_Publications](https://www.researchgate.net/publication/327942340_On_Reproducible_AI_Towards_Reproducible_Research_Open_Science_and_Digital_Scholarship_in_AI_Publications?enrichId=rgreq-d3eba7b3db33c9d191ea683f062934e7-XXX&enrichSource=Y292ZXJQYWdlOzMyNzk0MjM0MDtBUzo3NDE3MDU1NDg1NjI0MzJAMTU1Mzg0Nzc5MTA1Ng%3D%3D&el=1_x_2&_esc=publicationCoverPdf)
  Part I: Recommendations for data in publications.
  RECOMMENDATIONS 1-5: Data mentioned in a publication should:
  
  1. Be available in a shared community repository, so anyone can access it //
  2. Include basic metadata, so others can search and understand its contents//
  3. Have a license, so anyone can understand the conditions for reuse of the data //
  4. Have an associated digital object identifier (DOI) or persistent URL (PURL) so that the data is available permanently //
  5. Be cited properly in the prose and listed accurately among the references, so readers can identify the datasets unequivocally and data creators can receive credit for their work
  
  Part II: Recommendations for source code implementing AI methods and experiments in publications.
  RECOMMENDATIONS 6-10: Source code used for implementing an AI method and executing an experiment should
  
  6. Be available in a shared community repository, so anyone can access it
  7. Include basic metadata, so others can search and understand its contents
  8. Include a license, so anyone can understand the conditions for use and extension of the software
  9. Have an associated digital object identifier (DOI) or persistent URL (PURL) for the version used in the associated publication so that the source code is permanently available
  10. Be cited and referenced properly in the publication so that readers can identify the version unequivocally and its creators can receive credit for their work
  
  Part III: Recommendations for AI methods in publications.
  
  RECOMMENDATIONS (11-13): AI methods used in a publication should be:
  
  11. Presented in the context of a problem description that clearly identifies what problem they are intended to solve
  12. Outlined conceptually so that anyone can understand their foundational concepts
  13. Described in pseudocode so that others can understand the details of how they work
  
  Part IV: Recommendations for experiments described in publications.
  RECOMMENDATIONS (14-23): Descriptions of experiments in a publication should:
  
    14. Explicitly present the hypotheses to be assessed, before other details concerning the empirical study are presented
    15. Present the predicted outcome of the experiment, based on beliefs about the AI method and its application
    16. Include the experiment design (parameters and the conditions to be tested) and its motivation, such as why a specific number of tests or data points are used based on the desired statistical significance of results and the availability of data
    17. Identify and describe the measure and metrics
    18. Provide the evaluation protocol
    19. Share the results
    20. Describe the results and the analysis
    21. Be described as a workflow that summarizes how the experiment is executed and configured
    22. Include documentation on workflow executions or execution traces that provide parameter settings and initial, intermediate, and final data
    23. Specify the hardware used to run the experiments
    24. Be cited and published separately when complex, so that others can unequivocally refer to the individual portions of the method that they reuse or extend
        
- MICCAI : [https://aaai.org/conference/aaai/aaai-23/reproducibility-checklist/](https://miccai2021.org/files/downloads/MICCAI2021-Reproducibility-Checklist.pdf)

- AAAI: https://aaai.org/conference/aaai/aaai-23/reproducibility-checklist/

The considered mostly three points: <strong>code, method/implementation, and experiment</strong>









| **Theme**                                    | **On Reproducible AI**                               | **MICCAI**                                                         | **AAAI**                                              | **Notes**                                                                                                                  |
| -------------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Public availability of datasets**          | 1 (data in shared repo)                        | Dataset link if public                                             | Datasets publicly available (yes)                     | All emphasize *public access*. MICCAI & AAAI are conditional if data is not public, but First Source assumes it should be. |
| **Metadata for datasets**                    | 2 (basic metadata)                             | Dataset description, stats, cohort details, acquisition parameters | Detailed dataset description if not public            | MICCAI goes deeper into cohort, acquisition process, ethics; AAAI requires detail if not public.                           |
| **Licensing for datasets**                   | 3 (license)                                    | Not explicit                                                       | License for novel datasets (AAAI)                     | Only First Source & AAAI make licensing explicit; MICCAI doesn’t mention license.                                          |
| **Persistent identifier for datasets**       | 4 (DOI/PURL)                                   | Not explicit                                                       | Not explicit                                          | Only First Source explicitly calls for DOI/PURL.                                                                           |
| **Dataset citation in publications**         | 5 (cited properly)                             | Citation for existing datasets                                     | Citation for existing datasets                        | Shared principle: crediting dataset creators.                                                                              |
| **Public availability of code**              | 6 (repo)                                       | Code with link                                                     | Code public with license (yes)                        | All require sharing source code.                                                                                           |
| **Metadata for code**                        | 7 (metadata)                                   | Specification of dependencies, README                              | Not explicit as “metadata”, but lists dependencies    | MICCAI operationalizes metadata as dependencies; AAAI has pieces but no “metadata” term.                                   |
| **License for code**                         | 8 (license)                                    | Not explicit                                                       | License (yes)                                         | First Source & AAAI explicit; MICCAI omits.                                                                                |
| **Persistent identifier for code**           | 9 (DOI/PURL)                                   | Not explicit                                                       | Not explicit                                          | Only First Source explicit.                                                                                                |
| **Code citation**                            | 10 (cite & reference)                          | Not explicit                                                       | Not explicit                                          | First Source only.                                                                                                         |
| **Clear method description**                 | 11 (problem context) + 12 (conceptual outline) | Mathematical setting + explanation of assumptions                  | Conceptual outline (yes)                              | Same aim: clarity of purpose and conceptual structure.                                                                     |
| **Pseudocode**                               | 13                                             | Not explicit                                                       | Pseudocode (yes)                                      | First Source & AAAI explicit; MICCAI not.                                                                                  |
| **Hypotheses stated**                        | 14                                             | Not explicit                                                       | Clear separation of hypothesis/opinions/results (yes) | MICCAI doesn’t state hypothesis explicitly; AAAI includes in “clearly delineates hypotheses”.                              |
| **Predicted outcomes**                       | 15                                             | Not explicit                                                       | Not explicit                                          | Only First Source.                                                                                                         |
| **Experiment design & parameters**           | 16                                             | Hyper-parameter range, selection, all splits, baseline tuning      | All parameters tried, final parameters                | Strong overlap. MICCAI covers design via hyperparameters & splits; AAAI is very explicit on ranges & criteria.             |
| **Metrics definition**                       | 17                                             | Evaluation metrics defined                                         | Metrics defined + motivation                          | All cover this, AAAI adds justification for choice.                                                                        |
| **Evaluation protocol**                      | 18                                             | Train/val/test splits, baseline tuning                             | Methodology for runs, seeds, metrics                  | All include protocol-like details.                                                                                         |
| **Results reporting**                        | 19, 20                                         | Results with central tendency & variation                          | Results with variation & significance tests           | All require detailed result reporting, AAAI & MICCAI require significance testing.                                         |
| **Experiment workflow**                      | 21                                             | Not explicit                                                       | Not explicit                                          | Only First Source has “workflow” as a separate item.                                                                       |
| **Workflow documentation & traces**          | 22                                             | Not explicit                                                       | Not explicit                                          | Only First Source.                                                                                                         |
| **Hardware specification**                   | 23                                             | Computing infrastructure                                           | Hardware & software specs                             | All align here.                                                                                                            |
| **Separate publication for complex methods** | 24                                             | Not explicit                                                       | Not explicit                                          | Only First Source.                                                                                                         |
| **Dependencies & environment**               | (part of 7)                                    | Dependencies specified                                             | Names/versions of libraries/frameworks                | All cover environment setup.                                                                                               |
| **Pretrained models**                        | Not explicit                                   | Pretrained models provided                                         | Not explicit                                          | Only MICCAI.                                                                                                               |
| **Seed setting for reproducibility**         | Not explicit                                   | Not explicit                                                       | Seeds specified                                       | Only AAAI explicit.                                                                                                        |
| **Analysis of failures**                     | Not explicit                                   | Failure analysis                                                   | Not explicit                                          | Only MICCAI.                                                                                                               |
| **Energy/runtime/memory**                    | Not explicit                                   | Runtime, energy, memory footprint                                  | Not explicit                                          | Only MICCAI.                                                                                                               |
| **Ethics approval**                          | Not explicit                                   | Ethics statement if needed                                         | Not explicit                                          | Only MICCAI.                                                                                                               |
| **Clinical significance**                    | Not explicit                                   | Discussion of clinical significance                                | Not explicit                                          | Only MICCAI.                                                                                                               |

