===============

# Auto-Suggest: Learning-to-Recommend Data Preparation Steps Using Data Science Notebooks

 

## Overview

This benchmark dataset contains 78K real invocations of Pandas table-manipulation operators (Join, Pivot, Unpivot, GroupBy), harvested from replaying hundreds of thousands of notebooks publicly available on GitHub. We crawled over 4M notebooks, replayed a significant fraction of these notebooks by programmatically executing them, and used dynamic instrumentation to extract input-tables/parameters used by these aforementioned operators. 

 

We used this dataset to predict/recommend data-preparation steps (particularly for non-expert users) [1]. We hope the release of this data set would facilitate large-scale research on topics such as understanding the characteristics of real data manipulation tasks that data scientists perform in the wild; and building predictive models to automate data preparation tasks for expert and non-expert users alike.

## Data link

Data can be downloaded from [this link](https://onedrive.live.com/?authkey=!AGJdHNaO9kJuoLs&id=4EEA81351AF2D84B!7570&cid=4EEA81351AF2D84B). Each instance of an operator invocation is stored under a separate sub-folder with a structure of `[OPERATOR]/[GITREPO]_[FILEPATH]_cell[CELLID]_[OPERATORID]/`. Each sub-folder contains a `data.csv` for the input dataframe fed into the operator (dumped as a csv), and also a `param.json` for the exact parameters used in this invocation (the ground-truth we want to predict in [1]). 

## License

This data set is released under the [Computational Use of Data Agreement v1.0](https://github.com/microsoft/Computational-Use-of-Data-Agreement/blob/master/C-UDA-1.0.md). 

 

## Reference

[1] Auto-Suggest: Learning-to-Recommend Data Preparation Steps Using Data Science Notebooks. [https://dl.acm.org/doi/abs/10.1145/3318464.3389738](https://dl.acm.org/doi/abs/10.1145/3318464.3389738).

===============
