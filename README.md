# Deep learning illuminate’s hormonal biomarkers of Parkinson’s Disease
In this project, we provide a comprehensive set of tools for data preprocessing and modeling. The preprocessing stage is detailed in the notebook titled "Preprocessing_olink.ipynb", last updated on May 20, 2024. This notebook covers all necessary data cleaning, feature engineering, and transformations required for our analysis. Subsequently, we present three distinct modeling approaches, each implemented in separate notebooks. Firstly, the "OLINK_NN.ipynb" notebook implements an OLINK neural network model, utilizing the preprocessed data. Secondly, the "Ridge_witholink.ipynb" notebook employs Ridge regression, incorporating features derived from the OLINK preprocessing step. Lastly, the "SVM_Olink.ipynb" notebook introduces a Support Vector Machine model, leveraging the same set of OLINK features. All model notebooks have been updated with the latest code changes as of May 20, 2024. These notebooks collectively offer a comprehensive pipeline for data preprocessing and modeling, facilitating efficient analysis and experimentation. Users can refer to each notebook for detailed implementation, parameter tuning, and evaluation metrics. Additionally, instructions for usage and licensing information are provided for clarity and transparency. We extend our gratitude to all contributors and welcome any inquiries or collaboration opportunities.

**Abstract**
Introduction: Parkinson’s disease (PD) is a prevalent neurodegenerative disease marked by do-pamine loss in the striatum. New techniques for high throughput serum proteomics enable wider search of potential biomarkers for PD. Objective: We aim to identify potential biomarkers of PD and quantify their significance. Further, we map out pathway involvement of these biomarkers to gain insight into PD. Methods: We implemented three models including a neural network, ridge regression, and support vector machine. We take the top performing neural network and create sa-liency maps of the features using shapley additive explanations (SHAP) scores. Results: We identi-fied several hormonal features in our top feature set from SHAP scores results regarding the neu-ral network. Additionally, multiple pathways including JAK-STAT and PI3K-AKT are involved with statistically significant. Conclusions: Defined biomarkers indicate that a strong hormonal component associated with PD merits further investigation.


**CONTENT**:

-   [Variant plus Proteomic Models](#Variant-plus-Proteomic-Processing)
-   [Variant Only Models](#Variant-Only-Processing)
-   [Data Access](#data-access)

Scripts were written by Fayzan Chaudhry.

Please email us with questions related to the code.

Fayzan Chaudhry
[ffc4001\@med.cornell.edu](mailto:ffc4001@med.cornell.edu){.email}

![](WCM_MB_LOGO_HZSS1L_CLR_RGB.png) 
## Variant plus Proteomic Models

This repository houses a comprehensive collection of scripts and code dedicated to the analysis of proteomic data using advanced machine learning techniques. The primary focus is on implementing three distinct models: Support Vector Machine (SVM), Ridge Regression, and Neural Networks. Each model has been meticulously designed to handle the intricacies of proteomic data, enabling robust and accurate predictions. The SVM model leverages its ability to manage high-dimensional data and find optimal hyperplanes for classification tasks. Ridge Regression is employed to address potential multicollinearity in the dataset, ensuring more reliable coefficient estimates. Neural Networks, with their capability to capture non-linear relationships, are utilized to model complex patterns inherent in proteomic data. This multi-faceted approach allows for a comprehensive evaluation of different modeling techniques on the same dataset, providing valuable insights into their respective performance and suitability for proteomic analysis.

In addition to the machine learning models, the repository includes detailed preprocessing scripts essential for preparing the raw proteomic data for analysis. These scripts perform a variety of data cleaning tasks, such as handling missing values, and normalizing data distributions which are crucial for ensuring the quality and consistency of the dataset. By automating these preprocessing steps, the scripts facilitate a streamlined workflow, enabling researchers to focus on model development and evaluation. The combination of rigorous preprocessing and diverse machine learning models makes this repository a valuable resource for researchers and practitioners in the field of proteomics, offering a robust framework for data analysis and model comparison.

## Variant

This repository provides a comprehensive set of scripts and code for analyzing SNP (single nucleotide polymorphism) data using advanced machine learning models. The project focuses on three key models: Support Vector Machine (SVM), Ridge Regression, and Neural Networks, each optimized for the complexities of SNP data. Detailed preprocessing scripts are included. These preprocessing steps ensure data quality and consistency, streamlining the workflow for researchers to focus on model development and evaluation. This repository is a valuable resource for those working with SNP data, offering a robust framework for comprehensive data analysis and model comparison.

## Data Access

The easiest way to get started is to apply for UK Biobank and PPMI Data. Unfortunetly, we are not allowed to share data. 

### Software Packages

|                      |                      |                     |
|----------------------|----------------------|---------------------|
| Anndata 0.9.2         | Appnope 0.1.3 | argon2-cffi-bindings 21.2.0        |
| asttokens 2.2.1          | attrs23.1.0           |backcall0.2.0      |
| backports.functools-lru-cache1.6.4     | beautifulsoup44.12.2       | bleach6.0.0 |
| certifi2023.5.7 | cffi1.15.1  | charset-normalizer3.1.0 |
| click8.1.7 | cloudpickle2.2.1  | comm0.1.3 |
| contourpy1.0.7 | cycler0.11.0  |  debugpy1.6.7|
| decorator5.1.1 | defusedxml0.7.1  | entrypoints0.4 |
| executing1.2.0 |  fastjsonschema2.16.3 | filelock3.12.0 |
| flit_core3.8.0 | fonttools4.39.4 | get-annotations0.1.2 |
| h5py3.11.0 | idna3.4  | igraph0.11.4 |
| importlib-metadata6.6.0 | importlib-resources5.12.0  | ipykernel6.23.0 |
| ipython8.4.0 | ipython-genutils0.2.0  | ipywidgets8.0.6 |
|  jedi0.18.2| Jinja23.1.2  | joblib1.2.0 |
| jsonschema4.17.3 | jupyter1.0.0  | jupyter_client8.2.0 |
| jupyter-console6.6.3 |  jupyter_core5.3.0 | jupyter-events0.6.3 |
| jupyter_server2.5.0 | jupyter_server_terminals0.4.4  | jupyterlab-pygments0.2.2 |
|  jupyterlab-widgets3.0.7|  kiwisolver1.4.4 | llvmlite0.36.0 |
| loompy3.0.7 | MarkupSafe2.1.2  | matplotlib3.7.1 |
| matplotlib-inline0.1.6 | mistune2.0.5  | mpmath1.3.0 |
| natsort8.4.0 | nbclassic1.0.0  | nbclient0.7.4 |
| nbconvert7.4.0 | nbformat5.8.0  | nest-asyncio1.5.6 |
| networkx3.1 | notebook6.5.4  | notebook_shim0.2.3 |
|  numba0.53.0| numpy1.23.0  |  numpy-groupies0.9.22|
| packaging23.1 | pandocfilters1.5.0  | parso0.8.3 |
| patsy0.5.6 |  pexpect4.8.0 | pickleshare0.7.5 |
| Pillow9.5.0 | pip23.1.2  | pkgutil_resolve_name1.3.10 |
| platformdirs3.5.0 | ply3.11  | prometheus-client0.16.0 |
| prompt-toolkit3.0.38 | psutil5.9.5  | ptyprocess0.7.0 |
| pure-eval0.2.2 | pycparser2.21  | Pygments2.15.1 |
| pynndescent0.5.12 |  pyobjc-core9.1.1 | pyobjc-framework-Cocoa9.1.1 |
| pyparsing3.0.9 |  PyQt55.15.7 | PyQt5-sip12.11.0 |
| pyreadr0.4.7 | pyrsistent0.19.3  | python-dateutil2.8.2 |
| python-json-logger2.0.7 |  pytz2023.3 | PyYAML6.0 |
| pyzmq25.0.2 | qtconsole5.4.3  | QtPy2.3.1 |
| requests2.30.0 | rfc3339-validator0.1.4  | rfc3986-validator0.1.1 |
| scanpy1.9.8 | scikit-learn1.2.2  | scipy1.10.1 |
| scvelo0.3.2 | seaborn0.13.2  | Send2Trash1.8.2 |
| session-info1.0.0 |  setuptools67.7.2 | shap0.41.0 |
| sip6.7.9 | six1.16.0  | sklearn0.0.post5 |
|  slicer0.0.7| sniffio1.3.0  | soupsieve2.3.2.post1 |
| stack-data0.6.2 | statsmodels0.14.1  | stdlib-list0.10.0 |
| sympy1.12 | terminado0.17.1  | texttable1.7.0 |
| threadpoolctl3.1.0 | tinycss21.2.1  | toml0.10.2  |
| tomli2.0.1 |  torch2.0.1 | torchaudio2.0.2 |
| torchvision0.15.2 | tornado6.3  | tqdm4.65.0 |
| traitlets5.9.0 |  typing_extensions4.5.0 | tzdata2023.3 |
| umap-learn0.5.6 |  urllib32.0.2 | wcwidth0.2.6 |
| webencodings0.5.1 |  websocket-client1.5.1 | wheel0.40.0 |
| widgetsnbextension4.0.7 |  xgboost1.7.6 | zipp3.15.0 |
















