# CLEF HIPE 2020 results

We provide an **overview table** of the final results of the runs submitted by 13 teams for the HIPE shared task.

- Publication date: 12.06.2020.
- Bundles: 1 to 5
- Detailed results for all systems can be found in this .tsv file.
- Detailed results for each team's runs are sent privately.
- System name composition is: teamID_bundleID_LANG_runID.
- F1 scores below 0.01 are excluded from the table.
- Results are ordered by F1 scores.



### Teams

*(in numerical order)*

| Team key | Team name   | Team affiliation                                             |
| -------- | ----------- | ------------------------------------------------------------ |
| team1    | ehrmama     | University of Amsterdam, The Netherlands                     |
| team7    | IRISA       | IRISA, Rennes, France                                        |
| team8    | CISTeria    | Ludwig-Maximilians-Universität and Bayerische Staatsbibliothek München, Munich, Germany |
| team10   | L3i         | La Rochelle University, La Rochelle, France                  |
| team11   | NLP-UQAM    | Université du Quebec à Montréal, Montréal, Quebec            |
| team16   | ERTIM       | Inalco, Paris, France                                        |
| team23   | UPB         | Politehnica University of Bucharest, Bucarest, Bulgaria      |
| team28   | SinNER      | INRIA and Paris-Sorbonne University, Paris, France           |
| team31   | UvA.ILPS    | University of Amsterdam, Amsterdam, The Netherlands          |
| team33   | SBB         | Berlin State Library, Berlin, Germany                        |
| team37   | Inria-DeLFT | Almanach, Inria, Paris, France                               |
| team39   | LIMSI       | LIMSI, CNRS, Paris, France                                   |
| team40   | Webis       | Webis group, Bauhaus University Weimar, Germany              |



### About the evaluation (reminder)

NERC and Entity Linking (EL) are evaluated in terms of macro and micro Precision, Recall, F1-measure. Here only micro is reported.

- Evaluation scenarios for **NERC**
   - **Strict**: exact boundary matching.
   - **Fuzzy**: fuzzy boundary matching.

- Evaluation scenarios for **EL**:
In terms of boundaries, NEL is only evaluated according to the fuzzy setting in all scenarios. What is of interest is the capacity to provide the correct link rather than the correct boundaries (NERC task).
    - **Strict**: The system's top link prediction (NIL or QID) must be identical with the gold standard annotation.
    - **Relaxed**: The set of system's predictions is expanded with a set of historically related entities QIDs, e.g "Germany" is expended with the more specific "Confederation of the Rhine" and both are considered as valid answers. Systems are therefore evaluated more generously.  For this scenario, we additionally report F@1/3/5 in the .tsv files.

### 



<!--ts-->
   * [CLEF HIPE 2020 preliminary results](#clef-hipe-2020-preliminary-results)
      * [NERC coarse](#nerc-coarse)
         * [NERC coarse German strict (literal sense) [NE-COARSE-LIT-micro-strict]](#nerc-coarse-german-strict-literal-sense-ne-coarse-lit-micro-strict)
         * [NERC coarse German fuzzy (literal sense) [NE-COARSE-LIT-micro-fuzzy]](#nerc-coarse-german-fuzzy-literal-sense-ne-coarse-lit-micro-fuzzy)
         * [NERC coarse German strict (metonymic sense) [NE-COARSE-METO-micro-strict]](#nerc-coarse-german-strict-metonymic-sense-ne-coarse-meto-micro-strict)
         * [NERC coarse German fuzzy (metonymic sense) [NE-COARSE-METO-micro-fuzzy]](#nerc-coarse-german-fuzzy-metonymic-sense-ne-coarse-meto-micro-fuzzy)
         * [NERC coarse English strict (literal sense) [NE-COARSE-LIT-micro-strict]](#nerc-coarse-english-strict-literal-sense-ne-coarse-lit-micro-strict)
         * [NERC coarse English fuzzy (literal sense) [NE-COARSE-LIT-micro-fuzzy]](#nerc-coarse-english-fuzzy-literal-sense-ne-coarse-lit-micro-fuzzy)
         * [NERC coarse English strict (metonymic sense) [NE-COARSE-METO-micro-strict]](#nerc-coarse-english-strict-metonymic-sense-ne-coarse-meto-micro-strict)
         * [NERC coarse English fuzzy (metonymic sense) [NE-COARSE-METO-micro-fuzzy]](#nerc-coarse-english-fuzzy-metonymic-sense-ne-coarse-meto-micro-fuzzy)
         * [NERC coarse French strict (literal sense) [NE-COARSE-LIT-micro-strict]](#nerc-coarse-french-strict-literal-sense-ne-coarse-lit-micro-strict)
         * [NERC coarse French fuzzy (literal sense) [NE-COARSE-LIT-micro-fuzzy]](#nerc-coarse-french-fuzzy-literal-sense-ne-coarse-lit-micro-fuzzy)
         * [NERC coarse French strict (metonymic sense) [NE-COARSE-METO-micro-strict]](#nerc-coarse-french-strict-metonymic-sense-ne-coarse-meto-micro-strict)
         * [NERC coarse French fuzzy (metonymic sense) [NE-COARSE-METO-micro-fuzzy]](#nerc-coarse-french-fuzzy-metonymic-sense-ne-coarse-meto-micro-fuzzy)
      * [NERC fine](#nerc-fine)
         * [NERC fine German strict (literal sense) [NE-FINE-LIT-micro-strict]](#nerc-fine-german-strict-literal-sense-ne-fine-lit-micro-strict)
         * [NERC fine German fuzzy (literal sense) [NE-FINE-LIT-micro-fuzzy]](#nerc-fine-german-fuzzy-literal-sense-ne-fine-lit-micro-fuzzy)
         * [NERC fine German strict (metonymic sense) [NE-FINE-METO-micro-strict]](#nerc-fine-german-strict-metonymic-sense-ne-fine-meto-micro-strict)
         * [NERC fine German fuzzy (metonymic sense) [NE-FINE-METO-micro-fuzzy]](#nerc-fine-german-fuzzy-metonymic-sense-ne-fine-meto-micro-fuzzy)
         * [NERC fine German strict NE components [NE-FINE-COMP-micro-strict]](#nerc-fine-german-strict-ne-components-ne-fine-comp-micro-strict)
         * [NERC fine German fuzzy NE components [NE-FINE-COMP-micro-fuzzy]](#nerc-fine-german-fuzzy-ne-components-ne-fine-comp-micro-fuzzy)
         * [NERC fine German strict, nested entities [NE-NESTED-micro-strict]](#nerc-fine-german-strict-nested-entities-ne-nested-micro-strict)
         * [NERC fine German fuzzy, nested entities [NE-NESTED-micro-fuzzy]](#nerc-fine-german-fuzzy-nested-entities-ne-nested-micro-fuzzy)
         * [NERC fine French strict (literal sense) [NE-FINE-LIT-micro-strict]](#nerc-fine-french-strict-literal-sense-ne-fine-lit-micro-strict)
         * [NERC fine French fuzzy (literal sense) [NE-FINE-LIT-micro-fuzzy]](#nerc-fine-french-fuzzy-literal-sense-ne-fine-lit-micro-fuzzy)
         * [NERC fine French strict (metonymic sense) [NE-FINE-METO-micro-strict]](#nerc-fine-french-strict-metonymic-sense-ne-fine-meto-micro-strict)
         * [NERC fine French fuzzy (metonymic sense) [NE-FINE-METO-micro-fuzzy]](#nerc-fine-french-fuzzy-metonymic-sense-ne-fine-meto-micro-fuzzy)
         * [NERC fine French strict NE components [NE-FINE-COMP-micro-strict]](#nerc-fine-french-strict-ne-components-ne-fine-comp-micro-strict)
         * [NERC fine French fuzzy NE components [NE-FINE-COMP-micro-fuzzy]](#nerc-fine-french-fuzzy-ne-components-ne-fine-comp-micro-fuzzy)
         * [NERC fine French strict, nested entities [NE-NESTED-micro-strict]](#nerc-fine-french-strict-nested-entities-ne-nested-micro-strict)
         * [NERC fine French fuzzy, nested entities [NE-NESTED-micro-fuzzy]](#nerc-fine-french-fuzzy-nested-entities-ne-nested-micro-fuzzy)
      * [EL](#el)
         * [EL German strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-german-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL German strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-german-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL German relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-german-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL German relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-german-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)
         * [EL English strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-english-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL English strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-english-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL English relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-english-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL English relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-english-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)
         * [EL French strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-french-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL French strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-french-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL French relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-french-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL French relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-french-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)
      * [EL only](#el-only)
         * [EL only German strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-only-german-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL only German strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-only-german-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL only German relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-only-german-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL only German relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-only-german-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)
         * [EL only English strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-only-english-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL only English strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-only-english-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL only English relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-only-english-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL only English relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-only-english-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)
         * [EL only French strict @1 (literal sense) [NEL-LIT-micro-fuzzy-@1]](#el-only-french-strict-1-literal-sense-nel-lit-micro-fuzzy-1)
         * [EL only French strict @1 (metonymic sense) [NEL-METO-micro-fuzzy-@1]](#el-only-french-strict-1-metonymic-sense-nel-meto-micro-fuzzy-1)
         * [EL only French relaxed @1 (literal sense) [NEL-LIT-micro-fuzzy-relaxed-@1]](#el-only-french-relaxed-1-literal-sense-nel-lit-micro-fuzzy-relaxed-1)
         * [EL only French relaxed @1 (metonymic sense) [NEL-METO-micro-fuzzy-relaxed-@1]](#el-only-french-relaxed-1-metonymic-sense-nel-meto-micro-fuzzy-relaxed-1)

<!-- Added by: romanell, at: Tue Jun  9 18:18:54 CEST 2020 -->

<!--te-->


## NERC coarse

Relevant bundles: 1-4

### NERC coarse German strict (literal sense) \[`NE-COARSE-LIT-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2   | 0.797 | 0.79        | 0.805    |
| 2      | team10_bundle1_de_1   | 0.785 | 0.764       | 0.807    |
| 3      | team10_bundle1_de_3   | 0.785 | 0.764       | 0.807    |
| 4      | team1_bundle3_de_2    | 0.678 | 0.697       | 0.659    |
| 5      | team1_bundle3_de_1    | 0.671 | 0.693       | 0.65     |
| 6      | team28_bundle4_de_2   | 0.658 | 0.658       | 0.658    |
| 7      | team1_bundle3_de_3    | 0.653 | 0.658       | 0.648    |
| 8      | team8_bundle4_de_1    | 0.651 | 0.745       | 0.578    |
| 9      | team8_bundle4_de_2    | 0.649 | 0.744       | 0.576    |
| 10     | team28_bundle4_de_1   | 0.648 | 0.631       | 0.666    |
| 11     | team8_bundle4_de_3    | 0.642 | 0.738       | 0.568    |
| 12     | team23_bundle4_de_1   | 0.621 | 0.677       | 0.575    |
| 13     | team23_bundle4_de_2   | 0.618 | 0.638       | 0.6      |
| 14     | team31_bundle2_de_2   | 0.526 | 0.499       | 0.556    |
| 15     | team28_bundle4_de_3   | 0.521 | 0.644       | 0.438    |
| 16     | team33_bundle2_de_1   | 0.491 | 0.499       | 0.484    |
| 17     | baseline_bundle4_de_1 | 0.476 | 0.643       | 0.378    |
| 18     | team31_bundle2_de_1   | 0.459 | 0.406       | 0.527    |
| 19     | team40_bundle4_de_1   | 0.454 | 0.695       | 0.337    |
| 20     | team23_bundle4_de_3   | 0.224 | 0.178       | 0.302    |

### NERC coarse German fuzzy (literal sense) \[`NE-COARSE-LIT-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2   | 0.878 | 0.87        | 0.886    |
| 2      | team10_bundle1_de_1   | 0.861 | 0.838       | 0.886    |
| 3      | team10_bundle1_de_3   | 0.861 | 0.838       | 0.886    |
| 4      | team28_bundle4_de_1   | 0.796 | 0.775       | 0.819    |
| 5      | team1_bundle3_de_1    | 0.789 | 0.814       | 0.765    |
| 6      | team1_bundle3_de_2    | 0.784 | 0.807       | 0.763    |
| 7      | team28_bundle4_de_2   | 0.784 | 0.784       | 0.785    |
| 8      | team1_bundle3_de_3    | 0.781 | 0.787       | 0.775    |
| 9      | team8_bundle4_de_1    | 0.769 | 0.88        | 0.683    |
| 10     | team8_bundle4_de_2    | 0.768 | 0.88        | 0.682    |
| 11     | team8_bundle4_de_3    | 0.765 | 0.88        | 0.677    |
| 12     | team23_bundle4_de_2   | 0.763 | 0.788       | 0.74     |
| 13     | team23_bundle4_de_1   | 0.751 | 0.817       | 0.694    |
| 14     | team31_bundle2_de_2   | 0.726 | 0.689       | 0.768    |
| 15     | team33_bundle2_de_1   | 0.719 | 0.73        | 0.708    |
| 16     | team31_bundle2_de_1   | 0.697 | 0.618       | 0.8      |
| 17     | team28_bundle4_de_3   | 0.648 | 0.8         | 0.544    |
| 18     | baseline_bundle4_de_1 | 0.585 | 0.79        | 0.464    |
| 19     | team40_bundle4_de_1   | 0.545 | 0.833       | 0.405    |
| 20     | team23_bundle4_de_3   | 0.302 | 0.24        | 0.408    |

### NERC coarse German strict (metonymic sense) \[`NE-COARSE-METO-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2   | 0.634 | 0.571       | 0.712    |
| 2      | team10_bundle1_de_1   | 0.632 | 0.568       | 0.712    |
| 3      | team10_bundle1_de_3   | 0.632 | 0.568       | 0.712    |
| 4      | team1_bundle3_de_3    | 0.61  | 0.696       | 0.542    |
| 5      | team8_bundle4_de_1    | 0.596 | 0.738       | 0.5      |
| 6      | team8_bundle4_de_2    | 0.596 | 0.738       | 0.5      |
| 7      | team8_bundle4_de_3    | 0.596 | 0.738       | 0.5      |
| 8      | team1_bundle3_de_1    | 0.571 | 0.718       | 0.475    |
| 9      | team1_bundle3_de_2    | 0.571 | 0.718       | 0.475    |
| 10     | baseline_bundle4_de_1 | 0.435 | 0.814       | 0.297    |

### NERC coarse German fuzzy (metonymic sense) \[`NE-COARSE-METO-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2   | 0.694 | 0.626       | 0.78     |
| 2      | team10_bundle1_de_1   | 0.684 | 0.615       | 0.771    |
| 3      | team10_bundle1_de_3   | 0.684 | 0.615       | 0.771    |
| 4      | team8_bundle4_de_1    | 0.636 | 0.787       | 0.534    |
| 5      | team8_bundle4_de_2    | 0.636 | 0.787       | 0.534    |
| 6      | team8_bundle4_de_3    | 0.636 | 0.787       | 0.534    |
| 7      | team1_bundle3_de_3    | 0.619 | 0.707       | 0.551    |
| 8      | team1_bundle3_de_1    | 0.571 | 0.718       | 0.475    |
| 9      | team1_bundle3_de_2    | 0.571 | 0.718       | 0.475    |
| 10     | baseline_bundle4_de_1 | 0.435 | 0.814       | 0.297    |

### NERC coarse English strict (literal sense) \[`NE-COARSE-LIT-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_1   | 0.632 | 0.623       | 0.641    |
| 2      | team10_bundle1_en_3   | 0.626 | 0.617       | 0.635    |
| 3      | team10_bundle1_en_2   | 0.625 | 0.621       | 0.63     |
| 4      | team37_bundle4_en_1   | 0.524 | 0.461       | 0.606    |
| 5      | team31_bundle2_en_1   | 0.473 | 0.443       | 0.508    |
| 6      | team23_bundle4_en_1   | 0.463 | 0.522       | 0.416    |
| 7      | team23_bundle4_en_2   | 0.441 | 0.45        | 0.432    |
| 8      | baseline_bundle4_en_1 | 0.405 | 0.531       | 0.327    |
| 9      | team33_bundle2_en_1   | 0.327 | 0.347       | 0.31     |
| 10     | team1_bundle3_en_1    | 0.318 | 0.249       | 0.439    |
| 11     | team1_bundle3_en_2    | 0.313 | 0.257       | 0.401    |
| 12     | team40_bundle4_en_1   | 0.117 | 0.476       | 0.067    |
| 13     | team23_bundle4_en_3   | 0.077 | 0.054       | 0.134    |

### NERC coarse English fuzzy (literal sense) \[`NE-COARSE-LIT-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_3   | 0.806 | 0.794       | 0.817    |
| 2      | team10_bundle1_en_1   | 0.786 | 0.775       | 0.797    |
| 3      | team10_bundle1_en_2   | 0.78  | 0.774       | 0.786    |
| 4      | team31_bundle2_en_1   | 0.678 | 0.635       | 0.728    |
| 5      | team23_bundle4_en_1   | 0.659 | 0.743       | 0.592    |
| 6      | team37_bundle4_en_1   | 0.645 | 0.568       | 0.746    |
| 7      | team23_bundle4_en_2   | 0.634 | 0.647       | 0.621    |
| 8      | team33_bundle2_en_1   | 0.605 | 0.642       | 0.572    |
| 9      | baseline_bundle4_en_1 | 0.562 | 0.736       | 0.454    |
| 10     | team1_bundle3_en_2    | 0.494 | 0.405       | 0.633    |
| 11     | team1_bundle3_en_1    | 0.479 | 0.375       | 0.661    |
| 12     | team40_bundle4_en_1   | 0.215 | 0.873       | 0.122    |
| 13     | team23_bundle4_en_3   | 0.168 | 0.118       | 0.292    |

### NERC coarse English strict (metonymic sense) \[`NE-COARSE-METO-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_3   | 0.143 | 0.667       | 0.08     |
| 2      | team10_bundle1_en_2   | 0.121 | 0.25        | 0.08     |
| 3      | baseline_bundle4_en_1 | 0.077 | 1           | 0.04     |

### NERC coarse English fuzzy (metonymic sense) \[`NE-COARSE-METO-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_3   | 0.214 | 1           | 0.12     |
| 2      | team10_bundle1_en_2   | 0.182 | 0.375       | 0.12     |
| 3      | baseline_bundle4_en_1 | 0.077 | 1           | 0.04     |
| 4      | team33_bundle2_en_1   | 0.024 | 0.013       | 0.2      |

### NERC coarse French strict (literal sense) \[`NE-COARSE-LIT-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_2   | 0.84  | 0.831       | 0.849    |
| 2      | team10_bundle1_fr_1   | 0.831 | 0.823       | 0.839    |
| 3      | team10_bundle1_fr_3   | 0.831 | 0.823       | 0.839    |
| 4      | team39_bundle4_fr_2   | 0.814 | 0.799       | 0.829    |
| 5      | team39_bundle4_fr_3   | 0.807 | 0.798       | 0.818    |
| 6      | team39_bundle4_fr_1   | 0.801 | 0.791       | 0.811    |
| 7      | team28_bundle4_fr_2   | 0.795 | 0.788       | 0.802    |
| 8      | team28_bundle4_fr_1   | 0.786 | 0.778       | 0.794    |
| 9      | team1_bundle3_fr_2    | 0.778 | 0.793       | 0.764    |
| 10     | team1_bundle3_fr_3    | 0.767 | 0.776       | 0.757    |
| 11     | team1_bundle3_fr_1    | 0.757 | 0.754       | 0.761    |
| 12     | team23_bundle4_fr_2   | 0.689 | 0.693       | 0.686    |
| 13     | team31_bundle2_fr_2   | 0.686 | 0.656       | 0.719    |
| 14     | team23_bundle4_fr_1   | 0.684 | 0.715       | 0.656    |
| 15     | team7_bundle2_fr_2    | 0.668 | 0.705       | 0.634    |
| 16     | team7_bundle2_fr_3    | 0.668 | 0.705       | 0.634    |
| 17     | team7_bundle2_fr_1    | 0.652 | 0.697       | 0.612    |
| 18     | baseline_bundle4_fr_1 | 0.646 | 0.693       | 0.606    |
| 19     | team37_bundle4_fr_1   | 0.638 | 0.605       | 0.675    |
| 20     | team28_bundle4_fr_3   | 0.635 | 0.702       | 0.579    |
| 21     | team11_bundle4_fr_1   | 0.627 | 0.66        | 0.598    |
| 22     | team33_bundle2_fr_1   | 0.502 | 0.53        | 0.477    |
| 23     | team40_bundle4_fr_1   | 0.347 | 0.731       | 0.228    |
| 24     | team23_bundle4_fr_3   | 0.336 | 0.268       | 0.449    |
| 25     | team16_bundle1_fr_1   | 0.316 | 0.435       | 0.248    |

### NERC coarse French fuzzy (literal sense) \[`NE-COARSE-LIT-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_2   | 0.921 | 0.912       | 0.931    |
| 2      | team10_bundle1_fr_1   | 0.917 | 0.909       | 0.926    |
| 3      | team10_bundle1_fr_3   | 0.917 | 0.909       | 0.926    |
| 4      | team39_bundle4_fr_3   | 0.898 | 0.887       | 0.909    |
| 5      | team39_bundle4_fr_1   | 0.897 | 0.886       | 0.908    |
| 6      | team39_bundle4_fr_2   | 0.896 | 0.88        | 0.913    |
| 7      | team28_bundle4_fr_2   | 0.894 | 0.886       | 0.902    |
| 8      | team28_bundle4_fr_1   | 0.888 | 0.879       | 0.897    |
| 9      | team1_bundle3_fr_2    | 0.877 | 0.893       | 0.861    |
| 10     | team1_bundle3_fr_3    | 0.865 | 0.875       | 0.854    |
| 11     | team1_bundle3_fr_1    | 0.862 | 0.859       | 0.866    |
| 12     | team31_bundle2_fr_2   | 0.83  | 0.794       | 0.869    |
| 13     | team23_bundle4_fr_2   | 0.821 | 0.825       | 0.817    |
| 14     | team23_bundle4_fr_1   | 0.819 | 0.856       | 0.785    |
| 15     | team37_bundle4_fr_1   | 0.796 | 0.755       | 0.842    |
| 16     | team7_bundle2_fr_2    | 0.784 | 0.828       | 0.744    |
| 17     | team7_bundle2_fr_3    | 0.784 | 0.828       | 0.744    |
| 18     | baseline_bundle4_fr_1 | 0.769 | 0.825       | 0.721    |
| 19     | team7_bundle2_fr_1    | 0.769 | 0.823       | 0.722    |
| 20     | team28_bundle4_fr_3   | 0.763 | 0.844       | 0.697    |
| 21     | team11_bundle4_fr_1   | 0.756 | 0.796       | 0.72     |
| 22     | team33_bundle2_fr_1   | 0.725 | 0.765       | 0.689    |
| 23     | team16_bundle1_fr_1   | 0.439 | 0.604       | 0.344    |
| 24     | team40_bundle4_fr_1   | 0.416 | 0.876       | 0.273    |
| 25     | team23_bundle4_fr_3   | 0.414 | 0.331       | 0.554    |

### NERC coarse French strict (metonymic sense) \[`NE-COARSE-METO-micro-strict`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1   | 0.783 | 0.734       | 0.839    |
| 2      | team10_bundle1_fr_3   | 0.783 | 0.734       | 0.839    |
| 3      | team39_bundle4_fr_3   | 0.667 | 0.647       | 0.688    |
| 4      | team10_bundle1_fr_2   | 0.655 | 0.658       | 0.652    |
| 5      | team39_bundle4_fr_2   | 0.627 | 0.696       | 0.571    |
| 6      | team1_bundle3_fr_1    | 0.617 | 0.697       | 0.554    |
| 7      | team1_bundle3_fr_2    | 0.617 | 0.697       | 0.554    |
| 8      | team39_bundle4_fr_1   | 0.603 | 0.69        | 0.536    |
| 9      | team1_bundle3_fr_3    | 0.551 | 0.643       | 0.482    |
| 10     | team11_bundle4_fr_1   | 0.422 | 0.423       | 0.42     |
| 11     | baseline_bundle4_fr_1 | 0.268 | 0.541       | 0.179    |
| 12     | team33_bundle2_fr_1   | 0.004 | 0.002       | 0.027    |

### NERC coarse French fuzzy (metonymic sense) \[`NE-COARSE-METO-micro-fuzzy`\]

| Rank   | System                | F1    | Precision   | Recall   |
|:-------|:----------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1   | 0.783 | 0.734       | 0.839    |
| 2      | team10_bundle1_fr_3   | 0.783 | 0.734       | 0.839    |
| 3      | team39_bundle4_fr_3   | 0.675 | 0.655       | 0.696    |
| 4      | team10_bundle1_fr_2   | 0.673 | 0.676       | 0.67     |
| 5      | team39_bundle4_fr_2   | 0.637 | 0.707       | 0.58     |
| 6      | team1_bundle3_fr_1    | 0.627 | 0.708       | 0.562    |
| 7      | team1_bundle3_fr_2    | 0.627 | 0.708       | 0.562    |
| 8      | team39_bundle4_fr_1   | 0.603 | 0.69        | 0.536    |
| 9      | team1_bundle3_fr_3    | 0.582 | 0.679       | 0.509    |
| 10     | team11_bundle4_fr_1   | 0.466 | 0.468       | 0.464    |
| 11     | baseline_bundle4_fr_1 | 0.268 | 0.541       | 0.179    |

## NERC fine

Relevant bundles: 1, 3

### NERC fine German strict (literal sense) \[`NE-FINE-LIT-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_1 | 0.668 | 0.628       | 0.712    |
| 2      | team10_bundle1_de_3 | 0.668 | 0.628       | 0.712    |
| 3      | team10_bundle1_de_2 | 0.661 | 0.629       | 0.697    |
| 4      | team1_bundle3_de_2  | 0.62  | 0.65        | 0.592    |
| 5      | team1_bundle3_de_1  | 0.593 | 0.617       | 0.571    |
| 6      | team1_bundle3_de_3  | 0.57  | 0.583       | 0.558    |

### NERC fine German fuzzy (literal sense) \[`NE-FINE-LIT-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.771 | 0.734       | 0.813    |
| 2      | team10_bundle1_de_1 | 0.761 | 0.716       | 0.812    |
| 3      | team10_bundle1_de_3 | 0.761 | 0.716       | 0.812    |
| 4      | team1_bundle3_de_2  | 0.719 | 0.754       | 0.687    |
| 5      | team1_bundle3_de_1  | 0.689 | 0.717       | 0.663    |
| 6      | team1_bundle3_de_3  | 0.685 | 0.701       | 0.67     |

### NERC fine German strict (metonymic sense) \[`NE-FINE-METO-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.648 | 0.601       | 0.703    |
| 2      | team10_bundle1_de_1 | 0.636 | 0.58        | 0.703    |
| 3      | team10_bundle1_de_3 | 0.636 | 0.58        | 0.703    |
| 4      | team1_bundle3_de_3  | 0.619 | 0.707       | 0.551    |
| 5      | team1_bundle3_de_1  | 0.571 | 0.718       | 0.475    |
| 6      | team1_bundle3_de_2  | 0.571 | 0.718       | 0.475    |

### NERC fine German fuzzy (metonymic sense) \[`NE-FINE-METO-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.711 | 0.659       | 0.771    |
| 2      | team10_bundle1_de_1 | 0.682 | 0.622       | 0.754    |
| 3      | team10_bundle1_de_3 | 0.682 | 0.622       | 0.754    |
| 4      | team1_bundle3_de_3  | 0.629 | 0.717       | 0.559    |
| 5      | team1_bundle3_de_1  | 0.571 | 0.718       | 0.475    |
| 6      | team1_bundle3_de_2  | 0.571 | 0.718       | 0.475    |

### NERC fine German strict NE components \[`NE-FINE-COMP-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.642 | 0.595       | 0.698    |
| 2      | team10_bundle1_de_1 | 0.629 | 0.619       | 0.638    |
| 3      | team10_bundle1_de_3 | 0.629 | 0.619       | 0.638    |
| 4      | team1_bundle3_de_3  | 0.573 | 0.681       | 0.494    |
| 5      | team1_bundle3_de_1  | 0.536 | 0.7         | 0.434    |
| 6      | team1_bundle3_de_2  | 0.536 | 0.7         | 0.434    |

### NERC fine German fuzzy NE components \[`NE-FINE-COMP-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.707 | 0.654       | 0.768    |
| 2      | team10_bundle1_de_1 | 0.706 | 0.696       | 0.717    |
| 3      | team10_bundle1_de_3 | 0.706 | 0.696       | 0.717    |
| 4      | team1_bundle3_de_3  | 0.618 | 0.735       | 0.534    |
| 5      | team1_bundle3_de_1  | 0.576 | 0.753       | 0.466    |
| 6      | team1_bundle3_de_2  | 0.576 | 0.753       | 0.466    |

### NERC fine German strict, nested entities \[`NE-NESTED-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_1 | 0.513 | 0.471       | 0.562    |
| 2      | team10_bundle1_de_3 | 0.513 | 0.471       | 0.562    |
| 3      | team10_bundle1_de_2 | 0.403 | 0.49        | 0.342    |

### NERC fine German fuzzy, nested entities \[`NE-NESTED-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_1 | 0.562 | 0.517       | 0.616    |
| 2      | team10_bundle1_de_3 | 0.562 | 0.517       | 0.616    |
| 3      | team10_bundle1_de_2 | 0.484 | 0.588       | 0.411    |

### NERC fine French strict (literal sense) \[`NE-FINE-LIT-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_2 | 0.784 | 0.772       | 0.797    |
| 2      | team10_bundle1_fr_1 | 0.769 | 0.755       | 0.784    |
| 3      | team10_bundle1_fr_3 | 0.769 | 0.755       | 0.784    |
| 4      | team1_bundle3_fr_2  | 0.71  | 0.696       | 0.724    |
| 5      | team1_bundle3_fr_1  | 0.705 | 0.714       | 0.696    |
| 6      | team1_bundle3_fr_3  | 0.696 | 0.708       | 0.684    |
| 7      | team16_bundle1_fr_1 | 0.303 | 0.418       | 0.238    |

### NERC fine French fuzzy (literal sense) \[`NE-FINE-LIT-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_2 | 0.856 | 0.843       | 0.869    |
| 2      | team10_bundle1_fr_1 | 0.846 | 0.83        | 0.863    |
| 3      | team10_bundle1_fr_3 | 0.846 | 0.83        | 0.863    |
| 4      | team1_bundle3_fr_2  | 0.791 | 0.776       | 0.807    |
| 5      | team1_bundle3_fr_1  | 0.789 | 0.799       | 0.779    |
| 6      | team1_bundle3_fr_3  | 0.787 | 0.801       | 0.773    |
| 7      | team16_bundle1_fr_1 | 0.412 | 0.568       | 0.324    |

### NERC fine French strict (metonymic sense) \[`NE-FINE-METO-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.688 | 0.718       | 0.661    |
| 2      | team10_bundle1_fr_3 | 0.688 | 0.718       | 0.661    |
| 3      | team10_bundle1_fr_2 | 0.647 | 0.618       | 0.679    |
| 4      | team1_bundle3_fr_1  | 0.605 | 0.667       | 0.554    |
| 5      | team1_bundle3_fr_2  | 0.605 | 0.667       | 0.554    |
| 6      | team1_bundle3_fr_3  | 0.497 | 0.677       | 0.393    |

### NERC fine French fuzzy (metonymic sense) \[`NE-FINE-METO-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.707 | 0.738       | 0.679    |
| 2      | team10_bundle1_fr_3 | 0.707 | 0.738       | 0.679    |
| 3      | team10_bundle1_fr_2 | 0.655 | 0.626       | 0.688    |
| 4      | team1_bundle3_fr_1  | 0.605 | 0.667       | 0.554    |
| 5      | team1_bundle3_fr_2  | 0.605 | 0.667       | 0.554    |
| 6      | team1_bundle3_fr_3  | 0.497 | 0.677       | 0.393    |

### NERC fine French strict NE components \[`NE-FINE-COMP-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.705 | 0.68        | 0.732    |
| 2      | team10_bundle1_fr_3 | 0.705 | 0.68        | 0.732    |
| 3      | team10_bundle1_fr_2 | 0.693 | 0.661       | 0.728    |
| 4      | team1_bundle3_fr_3  | 0.662 | 0.695       | 0.632    |
| 5      | team1_bundle3_fr_1  | 0.657 | 0.7         | 0.618    |
| 6      | team1_bundle3_fr_2  | 0.657 | 0.7         | 0.618    |
| 7      | team16_bundle1_fr_1 | 0.043 | 0.042       | 0.045    |

### NERC fine French fuzzy NE components \[`NE-FINE-COMP-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.801 | 0.773       | 0.832    |
| 2      | team10_bundle1_fr_3 | 0.801 | 0.773       | 0.832    |
| 3      | team10_bundle1_fr_2 | 0.787 | 0.751       | 0.827    |
| 4      | team1_bundle3_fr_1  | 0.751 | 0.801       | 0.707    |
| 5      | team1_bundle3_fr_2  | 0.751 | 0.801       | 0.707    |
| 6      | team1_bundle3_fr_3  | 0.748 | 0.785       | 0.714    |
| 7      | team16_bundle1_fr_1 | 0.077 | 0.074       | 0.08     |

### NERC fine French strict, nested entities \[`NE-NESTED-micro-strict`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.367 | 0.337       | 0.402    |
| 2      | team10_bundle1_fr_3 | 0.367 | 0.337       | 0.402    |
| 3      | team10_bundle1_fr_2 | 0.354 | 0.333       | 0.378    |
| 4      | team1_bundle3_fr_1  | 0.329 | 0.397       | 0.28     |
| 5      | team1_bundle3_fr_2  | 0.329 | 0.397       | 0.28     |
| 6      | team1_bundle3_fr_3  | 0.254 | 0.327       | 0.207    |

### NERC fine French fuzzy, nested entities \[`NE-NESTED-micro-fuzzy`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.389 | 0.357       | 0.427    |
| 2      | team10_bundle1_fr_2 | 0.389 | 0.366       | 0.415    |
| 3      | team10_bundle1_fr_3 | 0.389 | 0.357       | 0.427    |
| 4      | team1_bundle3_fr_1  | 0.371 | 0.448       | 0.317    |
| 5      | team1_bundle3_fr_2  | 0.371 | 0.448       | 0.317    |
| 6      | team1_bundle3_fr_3  | 0.284 | 0.365       | 0.232    |

## EL

Relevant bundles: 1, 2

### EL German strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.534 | 0.531       | 0.538    |
| 2      | team10_bundle1_de_1 | 0.518 | 0.508       | 0.529    |
| 3      | team10_bundle1_de_3 | 0.515 | 0.502       | 0.528    |
| 4      | team33_bundle2_de_1 | 0.389 | 0.54        | 0.304    |
| 5      | team31_bundle2_de_1 | 0.258 | 0.245       | 0.272    |
| 6      | team31_bundle2_de_2 | 0.254 | 0.241       | 0.269    |

### EL German strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_1 | 0.396 | 0.324       | 0.508    |
| 2      | team10_bundle1_de_2 | 0.396 | 0.324       | 0.508    |
| 3      | team10_bundle1_de_3 | 0.383 | 0.308       | 0.508    |

### EL German relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_2 | 0.557 | 0.553       | 0.561    |
| 2      | team10_bundle1_de_1 | 0.541 | 0.53        | 0.552    |
| 3      | team10_bundle1_de_3 | 0.537 | 0.524       | 0.55     |
| 4      | team33_bundle2_de_1 | 0.403 | 0.561       | 0.315    |
| 5      | team31_bundle2_de_1 | 0.268 | 0.255       | 0.283    |
| 6      | team31_bundle2_de_2 | 0.264 | 0.25        | 0.279    |

### EL German relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_de_1 | 0.469 | 0.384       | 0.602    |
| 2      | team10_bundle1_de_2 | 0.469 | 0.384       | 0.602    |
| 3      | team10_bundle1_de_3 | 0.454 | 0.364       | 0.602    |

### EL English strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_3 | 0.531 | 0.523       | 0.539    |
| 2      | team10_bundle1_en_1 | 0.523 | 0.514       | 0.533    |
| 3      | team10_bundle1_en_2 | 0.501 | 0.496       | 0.506    |
| 4      | team31_bundle2_en_1 | 0.3   | 0.249       | 0.375    |
| 5      | team33_bundle2_en_1 | 0.141 | 0.257       | 0.097    |

### EL English strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_1 | 0.185 | 0.172       | 0.2      |
| 2      | team10_bundle1_en_2 | 0.049 | 0.062       | 0.04     |
| 3      | team10_bundle1_en_3 | 0.048 | 0.059       | 0.04     |

### EL English relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_3 | 0.531 | 0.523       | 0.539    |
| 2      | team10_bundle1_en_1 | 0.523 | 0.514       | 0.533    |
| 3      | team10_bundle1_en_2 | 0.501 | 0.496       | 0.506    |
| 4      | team31_bundle2_en_1 | 0.3   | 0.249       | 0.375    |
| 5      | team33_bundle2_en_1 | 0.141 | 0.257       | 0.097    |

### EL English relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_en_1 | 0.185 | 0.172       | 0.2      |
| 2      | team10_bundle1_en_2 | 0.049 | 0.062       | 0.04     |
| 3      | team10_bundle1_en_3 | 0.048 | 0.059       | 0.04     |

### EL French strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_3 | 0.598 | 0.594       | 0.602    |
| 2      | team10_bundle1_fr_1 | 0.597 | 0.592       | 0.601    |
| 3      | team10_bundle1_fr_2 | 0.597 | 0.592       | 0.602    |
| 4      | team7_bundle2_fr_2  | 0.421 | 0.446       | 0.399    |
| 5      | team7_bundle2_fr_1  | 0.419 | 0.45        | 0.393    |
| 6      | team7_bundle2_fr_3  | 0.413 | 0.437       | 0.391    |
| 7      | team33_bundle2_fr_1 | 0.407 | 0.594       | 0.31     |
| 8      | team31_bundle2_fr_2 | 0.251 | 0.352       | 0.195    |
| 9      | team16_bundle1_fr_1 | 0.108 | 0.15        | 0.084    |

### EL French strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.297 | 0.236       | 0.402    |
| 2      | team10_bundle1_fr_3 | 0.297 | 0.236       | 0.402    |
| 3      | team10_bundle1_fr_2 | 0.265 | 0.217       | 0.339    |
| 4      | team7_bundle2_fr_3  | 0.043 | 0.023       | 0.295    |
| 5      | team7_bundle2_fr_2  | 0.041 | 0.022       | 0.286    |
| 6      | team7_bundle2_fr_1  | 0.037 | 0.02        | 0.25     |

### EL French relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.617 | 0.612       | 0.621    |
| 2      | team10_bundle1_fr_2 | 0.617 | 0.612       | 0.622    |
| 3      | team10_bundle1_fr_3 | 0.617 | 0.613       | 0.622    |
| 4      | team7_bundle2_fr_2  | 0.439 | 0.465       | 0.417    |
| 5      | team7_bundle2_fr_1  | 0.438 | 0.47        | 0.41     |
| 6      | team7_bundle2_fr_3  | 0.432 | 0.457       | 0.409    |
| 7      | team33_bundle2_fr_1 | 0.422 | 0.616       | 0.321    |
| 8      | team31_bundle2_fr_2 | 0.252 | 0.353       | 0.196    |
| 9      | team16_bundle1_fr_1 | 0.108 | 0.15        | 0.084    |

### EL French relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System              | F1    | Precision   | Recall   |
|:-------|:--------------------|:------|:------------|:---------|
| 1      | team10_bundle1_fr_1 | 0.462 | 0.366       | 0.625    |
| 2      | team10_bundle1_fr_3 | 0.462 | 0.366       | 0.625    |
| 3      | team10_bundle1_fr_2 | 0.418 | 0.343       | 0.536    |
| 4      | team7_bundle2_fr_3  | 0.076 | 0.041       | 0.527    |
| 5      | team7_bundle2_fr_2  | 0.075 | 0.041       | 0.518    |
| 6      | team7_bundle2_fr_1  | 0.072 | 0.039       | 0.482    |

## EL only

Relevant bundles: 5

### EL only German strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_de_3             | 0.582 | 0.581       | 0.582    |
| 2      | team10_bundle5_de_1             | 0.565 | 0.565       | 0.564    |
| 3      | team10_bundle5_de_2             | 0.564 | 0.564       | 0.563    |
| 4      | team33_bundle5_de_1             | 0.445 | 0.615       | 0.349    |
| 5      | aidalight-baseline_bundle5_de_1 | 0.418 | 0.42        | 0.416    |

### EL only German strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_de_1             | 0.519 | 0.443       | 0.627    |
| 2      | team10_bundle5_de_2             | 0.519 | 0.443       | 0.627    |
| 3      | team10_bundle5_de_3             | 0.505 | 0.431       | 0.61     |
| 4      | aidalight-baseline_bundle5_de_1 | 0.31  | 0.265       | 0.373    |

### EL only German relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_de_3             | 0.602 | 0.601       | 0.602    |
| 2      | team10_bundle5_de_1             | 0.587 | 0.588       | 0.587    |
| 3      | team10_bundle5_de_2             | 0.586 | 0.587       | 0.586    |
| 4      | team33_bundle5_de_1             | 0.461 | 0.636       | 0.361    |
| 5      | aidalight-baseline_bundle5_de_1 | 0.437 | 0.44        | 0.435    |

### EL only German relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_de_1             | 0.604 | 0.515       | 0.729    |
| 2      | team10_bundle5_de_2             | 0.604 | 0.515       | 0.729    |
| 3      | team10_bundle5_de_3             | 0.568 | 0.485       | 0.686    |
| 4      | aidalight-baseline_bundle5_de_1 | 0.387 | 0.331       | 0.466    |

### EL only English strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team37_bundle5_en_1             | 0.658 | 0.633       | 0.685    |
| 2      | team10_bundle5_en_1             | 0.593 | 0.593       | 0.593    |
| 3      | team10_bundle5_en_2             | 0.593 | 0.593       | 0.593    |
| 4      | team31_bundle5_en_3             | 0.593 | 0.607       | 0.58     |
| 5      | team10_bundle5_en_3             | 0.58  | 0.58        | 0.58     |
| 6      | aidalight-baseline_bundle5_en_1 | 0.506 | 0.506       | 0.506    |
| 7      | team31_bundle5_en_1             | 0.367 | 0.365       | 0.369    |
| 8      | team31_bundle5_en_2             | 0.348 | 0.344       | 0.353    |
| 9      | team33_bundle5_en_1             | 0.177 | 0.344       | 0.119    |

### EL only English strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_en_1             | 0.358 | 0.286       | 0.48     |
| 2      | team10_bundle5_en_2             | 0.358 | 0.286       | 0.48     |
| 3      | team10_bundle5_en_3             | 0.358 | 0.286       | 0.48     |
| 4      | aidalight-baseline_bundle5_en_1 | 0.246 | 0.219       | 0.28     |
| 5      | team31_bundle5_en_3             | 0.058 | 0.031       | 0.52     |

### EL only English relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team37_bundle5_en_1             | 0.658 | 0.633       | 0.685    |
| 2      | team10_bundle5_en_1             | 0.593 | 0.593       | 0.593    |
| 3      | team10_bundle5_en_2             | 0.593 | 0.593       | 0.593    |
| 4      | team31_bundle5_en_3             | 0.593 | 0.607       | 0.58     |
| 5      | team10_bundle5_en_3             | 0.58  | 0.58        | 0.58     |
| 6      | aidalight-baseline_bundle5_en_1 | 0.506 | 0.506       | 0.506    |
| 7      | team31_bundle5_en_1             | 0.367 | 0.365       | 0.369    |
| 8      | team31_bundle5_en_2             | 0.348 | 0.344       | 0.353    |
| 9      | team33_bundle5_en_1             | 0.177 | 0.344       | 0.119    |

### EL only English relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_en_1             | 0.358 | 0.286       | 0.48     |
| 2      | team10_bundle5_en_2             | 0.358 | 0.286       | 0.48     |
| 3      | team10_bundle5_en_3             | 0.358 | 0.286       | 0.48     |
| 4      | aidalight-baseline_bundle5_en_1 | 0.246 | 0.219       | 0.28     |
| 5      | team31_bundle5_en_3             | 0.058 | 0.031       | 0.52     |
| 6      | team31_bundle5_en_1             | 0.008 | 0.004       | 0.08     |
| 7      | team31_bundle5_en_2             | 0.004 | 0.002       | 0.04     |

### EL only French strict @1 (literal sense) \[`NEL-LIT-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_fr_1             | 0.639 | 0.64        | 0.638    |
| 2      | team10_bundle5_fr_2             | 0.633 | 0.635       | 0.632    |
| 3      | team10_bundle5_fr_3             | 0.632 | 0.633       | 0.63     |
| 4      | team37_bundle5_fr_1             | 0.616 | 0.585       | 0.65     |
| 5      | aidalight-baseline_bundle5_fr_1 | 0.498 | 0.502       | 0.495    |
| 6      | team33_bundle5_fr_1             | 0.48  | 0.677       | 0.371    |
| 7      | team7_bundle5_fr_1              | 0.474 | 0.475       | 0.473    |
| 8      | team7_bundle5_fr_3              | 0.463 | 0.464       | 0.461    |
| 9      | team7_bundle5_fr_2              | 0.436 | 0.438       | 0.435    |

### EL only French strict @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_fr_1             | 0.361 | 0.303       | 0.446    |
| 2      | team10_bundle5_fr_2             | 0.361 | 0.303       | 0.446    |
| 3      | team10_bundle5_fr_3             | 0.354 | 0.297       | 0.438    |
| 4      | aidalight-baseline_bundle5_fr_1 | 0.254 | 0.213       | 0.312    |
| 5      | team7_bundle5_fr_3              | 0.047 | 0.025       | 0.357    |
| 6      | team7_bundle5_fr_1              | 0.04  | 0.021       | 0.304    |
| 7      | team7_bundle5_fr_2              | 0.04  | 0.021       | 0.304    |

### EL only French relaxed @1 (literal sense) \[`NEL-LIT-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_fr_1             | 0.659 | 0.66        | 0.657    |
| 2      | team10_bundle5_fr_2             | 0.653 | 0.654       | 0.652    |
| 3      | team10_bundle5_fr_3             | 0.652 | 0.653       | 0.65     |
| 4      | team37_bundle5_fr_1             | 0.635 | 0.604       | 0.67     |
| 5      | aidalight-baseline_bundle5_fr_1 | 0.512 | 0.516       | 0.508    |
| 6      | team33_bundle5_fr_1             | 0.495 | 0.699       | 0.383    |
| 7      | team7_bundle5_fr_1              | 0.492 | 0.492       | 0.491    |
| 8      | team7_bundle5_fr_3              | 0.484 | 0.486       | 0.482    |
| 9      | team7_bundle5_fr_2              | 0.454 | 0.455       | 0.452    |

### EL only French relaxed @1 (metonymic sense) \[`NEL-METO-micro-fuzzy-relaxed-@1`\]

| Rank   | System                          | F1    | Precision   | Recall   |
|:-------|:--------------------------------|:------|:------------|:---------|
| 1      | team10_bundle5_fr_1             | 0.549 | 0.461       | 0.679    |
| 2      | team10_bundle5_fr_2             | 0.549 | 0.461       | 0.679    |
| 3      | team10_bundle5_fr_3             | 0.542 | 0.455       | 0.67     |
| 4      | aidalight-baseline_bundle5_fr_1 | 0.384 | 0.323       | 0.473    |
| 5      | team7_bundle5_fr_3              | 0.076 | 0.041       | 0.58     |
| 6      | team7_bundle5_fr_1              | 0.07  | 0.038       | 0.536    |
| 7      | team7_bundle5_fr_2              | 0.069 | 0.037       | 0.527    |
