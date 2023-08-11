# DLPEA
The code 
# Datasets
源代码是在OpenEA框架的基础上实现的，我们遵循OpenEA相同的设计特点来实现功能，同时保持可扩展性。我们在实现中保留了OpenEA的部分，列出了以下的源代码（连同注释）。
# code<br>
“|__ run<br>
|   |__ args<br>
|   |   |__ args_15K.json    // config file for 15K benchmark<br>
|   |   |__ args_100K.json   // config file for 100K benchmark<br>
|   |__ main_from_args.py           // interface with args input<br>
|   |__ run_DLPEA.sh               // bash script to run experiments<br>
|__ src<br>
|   |__ openea<br>
|   |   |__ approaches<br>
|   |   |   |__ DLPEA.py           // DLPEAEA core code<br>
|   |   |__ models<br>
|   |   |   |__ basic_model.py      // same as OpenEA<br>
|   |   |__ modules<br>
|   |   |   |__ args<br>
|   |   |   |   |__ args_hander.py  // same as OpenEA<br>
|   |   |   |__ base<br>
|   |   |   |   |__ initializers.py // same as OpenEA<br>
|   |   |   |   |__ losses.py       // same as OpenEA<br>
|   |   |   |   |__ mapping.py      // same as OpenEA (with minor updates)<br>
|   |   |   |   |__ optimizers.py   // same as OpenEA<br>
|   |   |   |__ finding<br>
|   |   |   |   |__ alignment.py    // same as OpenEA<br>
|   |   |   |   |__ evaluation.py   // same as OpenEA (with minor updates)<br>
|   |   |   |   |__ similarity.py   // same as OpenEA<br>
|   |   |   |__ load<br>
|   |   |   |   |__ kg.py           // same as OpenEA<br>
|   |   |   |   |__ kgs.py          // same as OpenEA (with updates)<br>
|   |   |   |   |__ read.py         // same as OpenEA (with updates)<br>
|   |   |   |__ train<br>
|   |   |   |   |__ batch.py        // same as OpenEA (with minor updates)<br>
|   |   |   |   |__ sample.py       // same as OpenEA (with minor updates)<br>
|   |   |   |__ utils<br>
|   |   |   |   |__ check.py        // same as OpenEA (with updates)<br>
|   |   |   |   |__ inference.py    // same as OpenEA (with updates)<br>
|   |   |   |   |__ util.py         // same as OpenEA”<br>

# 如何运行
由于我们采用OpenEA代码库来实现DLPA，运行的方式与使用OpenEA的方式非常相似。

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
