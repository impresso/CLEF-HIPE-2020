# HIPE Shared Task Data

This folder contains the data releases relative to the [CLEF-HIPE shared task](https://impresso.github.io/CLEF-HIPE-2020/) on NERC and EL on historical newspapers. Please note that these datasets are not yet in their final versions but will evolve until end of spring 2020 approximately.


- **test-masked-v1.3** (released 03.06.2020): masked test dataset for evaluation of system runs for task bundle 5.
- **test-masked-v1.2** (released 25.05.2020): masked test dataset for evaluation of system runs for task bundles 1-4.
- **training-v1.2**  (released 12.10.2020): fourth version of training and dev datasets for HIP. Main changes are: additional data for French and German.
- **training-v1.1**  (released 7.04.2020): this release fixes a problem in the German validation set (see issue [#5](https://github.com/impresso/CLEF-HIPE-2020/issues/5)), as well as with escaping double quotes in the TSV exports.
- **training-v1.0** (released 26.03.2020): second version of training and dev datasets for German and French, and of dev dataset for English (there won't be training data for English). Main changes are quantitative (more documents and therefore more mentions and linked entities). Foreseen release v1.1 beginning of april with increased quality.
- **training-v0.9** (released 20.02.2020): first version of training and dev datasets for German and French, and first version of dev dataset for English (there won't be training data for English). 


- **sample-v1.0** (released 10.01.2020): 10 French and 8 German content items fully annotated.



### License

The HIPE datasets are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a> 


### How to cite

If you use this data, please consider citing the CLEF-HIPE-2020 overview papers:


CEUR Extended overview: [https://infoscience.epfl.ch/record/281054](https://infoscience.epfl.ch/record/281054)

```
@inproceedings{ehrmann_extended_2020,
  title = {Extended {Overview} of {CLEF HIPE} 2020: {Named Entity Processing} on {Historical Newspapers}},
  booktitle = {{CLEF 2020 Working Notes}. {Working Notes} of {CLEF} 2020 - {Conference} and {Labs} of the {Evaluation Forum}},
  author = {Ehrmann, Maud and Romanello, Matteo and Fl{\"u}ckiger, Alex and Clematide, Simon},
  editor = {Cappellato, Linda and Eickhoff, Carsten and Ferro, Nicola and N{\'e}v{\'e}ol, Aur{\'e}lie},
  year = {2020},
  volume = {2696},
  pages = {38},
  publisher = {{CEUR-WS}},
  address = {{Thessaloniki, Greece}},
  doi = {10.5281/zenodo.4117566},
  url = {https://infoscience.epfl.ch/record/281054},
}
```

or Springer LNCS overview: [https://link.springer.com/chapter/10.1007/978-3-030-58219-7_21](https://link.springer.com/chapter/10.1007/978-3-030-58219-7_21)

```
@InProceedings{10.1007/978-3-030-58219-7_21,
author="Ehrmann, Maud and Romanello, Matteo and Fl{\"u}ckiger, Alex and Clematide, Simon",
editor="Arampatzis, Avi and Kanoulas, Evangelos and Tsikrika, Theodora and Vrochidis, Stefanos and Joho, Hideo and Lioma, Christina and Eickhoff, Carsten and N{\'e}v{\'e}ol, Aur{\'e}lie and Cappellato, Linda and Ferro, Nicola",
title="Overview of CLEF HIPE 2020: Named Entity Recognition and Linking on Historical Newspapers",
booktitle="Experimental IR Meets Multilinguality, Multimodality, and Interaction",
year="2020",
publisher="Springer International Publishing",
address="Cham",
pages="288--310",
isbn="978-3-030-58219-7"
}

```
Results of participating teams appear in the working notes proceedings, published by [CEUR Workshop](http://ceur-ws.org/), and were presented in the CLEF conference in Sept 2020 (see [youtube](https://www.youtube.com/playlist?list=PLB45F159nVx-3bee7G_1jdTfUAtsLD0FU) playlist). 



