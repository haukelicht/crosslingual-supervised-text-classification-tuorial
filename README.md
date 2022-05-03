# Cross-lingual supervised text classification


<center>
<b style="font-size: 150%">Hauke Licht</b>
<br>
<em style="font-size: 120%">Cologne Center for Comparative Politics, University of Cologne</em>
<br>
<a href="mailto:hauke.licht@wiso.uni-koeln.de">hauke.licht@wiso.uni-koeln.de</a>
</center>
<br style="margin-below: 12pt;">

This repository contains the slides for my short tutorial on *cross-lingual supervised text classification* I have prepared for the [COMPTEXT 2022 conference](https://www.comptextconference.org/4th-annual-comptext-conference-2022/).

Below, you find the links to the data and interactive Google Colab notebooks I use during the tutorial:

| Link | Description |
|:---- |:----- |
| [file](https://drive.google.com/file/d/1dvEh-p-uOPciJSe56Wqg25ji6S9kK_HQ/view?usp=sharing) | This CSV file is a cleaned version of the data set compiled by [Pola Lehmann and Malisa Zobel (2018)](https://doi.org/10.1111/1475-6765.12266). The file can be downloaded or read from my Google Drive. *Note:* that the data already records machine-translated versions of sentences' original texts. |
| [notebook](https://colab.research.google.com/drive/15tgAUdM_zyNiD5i_aQsi4FAK8YBLbFy1?usp=sharing) | This notebook is a short walk through through the Lehmann+Zobel data that reports on the label and language distribution in the data. |
| [notebook](https://colab.research.google.com/drive/1wOcGrYVQP1xphhzh9_xr_Fjlk9F5oJyc?usp=sharing) | In this notebook I use the Lehmann+Zobel data as an example to show how to use the [`easyNMT` python package](https://github.com/UKPLab/EasyNMT) to machine-translate a multilingual corpus free of charge. |
| [notebook](https://colab.research.google.com/drive/1twzysCOemnXQ17A10FZvbJ86DeyIiNGm?usp=sharing) | In this notebook I use the Lehmann+Zobel data as an example to show how to use the [`sentence-transformers` python package](https://www.sbert.net/examples/training/multilingual/README.html) to sentence-embed documents in a multilingual corpus. |
| [folder](https://drive.google.com/drive/folders/1CnoQBBvK4HiE1nGkSDWNFOCAHSscTam0?usp=sharing) | This contain in my Google Drive records zipped TSV files that records multilingual sentence embeddings of the sentences in the Lehmann+Zobel data I have generated using the knowledge-distilled XLM-R model available through the `sentence-transformers` package. The folder can be downloaded or read from my Google Drive. |
| [notebook](https://colab.research.google.com/drive/1s31bJRpB4GizBIFQ1N6hhI9lc-PVY8kM?usp=sharing) | In this notebook I sample quasi-sentences in the Lehmann+Zobel data into training, test, and cross validation folds. |
| [file](https://drive.google.com/file/d/1GVPIJzhjXJt0zQJrR_3rdi5QVIkuhpF7/view?usp=sharing) | This JSON file records the training, test, and cross validation indeces sampled in the notebook described above. The file can be downloaded or read from my Google Drive.|
| [notebook](https://colab.research.google.com/drive/1Uwp3WZpVTrybj4nqK6zGeGE1eTJnUP6D?usp=sharing) | In this notebook I train and evaluate supervised text classifiers on bag-of-word representations on machince-translated versions of quasi-sentences in the Lehmann+Zobel data. |
| [notebook](https://colab.research.google.com/drive/1K8mrFCOACKZvoVRa9qqZwVfyCpIWbJEl?usp=sharing) | In this notebook I train and evaluate supervised text classifiers using multilingual sentence embeddings of quasi-sentences in the Lehmann+Zobel data. |
| [notebook](https://colab.research.google.com/drive/1RKyJwxeBUCh03PGj2nOR_cxPqS0u3utz?usp=sharing) | In this notebook I assess language independence of an MSE-based classifier trained on quasi-sentences in the Lehmann+Zobel data. |

*Note:* If you haven't worked with Google Colab notebooks before, check out [this](https://colab.research.google.com/?utm_source=scs-index) short tutorial