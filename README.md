# DLPEA
The code of "基于动态图注意力与标签传播的实体对齐"
# Datasets
源代码是在OpenEA框架的基础上实现的，我们遵循OpenEA相同的设计特点来实现功能，同时保持可扩展性。我们在实现中保留了OpenEA的部分，列出了以下的源代码（连同注释）。
# code
“|__ run
|   |__ args
|   |   |__ args_15K.json    // config file for 15K benchmark
|   |   |__ args_100K.json   // config file for 100K benchmark
|   |__ main_from_args.py           // interface with args input
|   |__ run_DLPEA.sh               // bash script to run experiments
|__ src
|   |__ openea
|   |   |__ approaches
|   |   |   |__ DLPEA.py           // DLPEAEA core code
|   |   |__ models
|   |   |   |__ basic_model.py      // same as OpenEA
|   |   |__ modules
|   |   |   |__ args
|   |   |   |   |__ args_hander.py  // same as OpenEA
|   |   |   |__ base
|   |   |   |   |__ initializers.py // same as OpenEA
|   |   |   |   |__ losses.py       // same as OpenEA
|   |   |   |   |__ mapping.py      // same as OpenEA (with minor updates)
|   |   |   |   |__ optimizers.py   // same as OpenEA
|   |   |   |__ finding
|   |   |   |   |__ alignment.py    // same as OpenEA
|   |   |   |   |__ evaluation.py   // same as OpenEA (with minor updates)
|   |   |   |   |__ similarity.py   // same as OpenEA
|   |   |   |__ load
|   |   |   |   |__ kg.py           // same as OpenEA
|   |   |   |   |__ kgs.py          // same as OpenEA (with updates)
|   |   |   |   |__ read.py         // same as OpenEA (with updates)
|   |   |   |__ train
|   |   |   |   |__ batch.py        // same as OpenEA (with minor updates)
|   |   |   |   |__ sample.py       // same as OpenEA (with minor updates)
|   |   |   |__ utils
|   |   |   |   |__ check.py        // same as OpenEA (with updates)
|   |   |   |   |__ inference.py    // same as OpenEA (with updates)
|   |   |   |   |__ util.py         // same as OpenEA”

# 如何运行
由于我们采用OpenEA代码库来实现DLPA，运行的方式与使用OpenEA的方式非常相似。
更具体的复现之后会放出
# Dependencies
Scipy
Pandas
Scikit-learn
Gensim
tensorflow == 2.6.0
Python == 3.7.0
faiss
Numpy
tqdm
pickle
