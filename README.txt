激活conda环境：
conda activate opennmt

获取vocabulary包：
onmt_build_vocab -config {conifg.yaml} -n_sample {20000}

训练：
onmt_train -config {config.yaml}

使用模型翻译：
onmt_translate -model {PATH TO model.pt} -src {PATH TO src.txt} -output {PATH TO ouput.txt} -gpu 0 -verbose