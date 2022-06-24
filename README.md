# Error Templates for Grammatical Error Correction
Code for the paper: "[Mining Error Templates for Grammatical Error Correction](https://arxiv.org/abs/2206.11569)". If you use any part of this work, please cite our paper:
```
@article{zhang2022templates,
  title={Mining Error Templates for Grammatical Error Correction}, 
  author={Yue Zhang and Haochen Jiang and Zuyi Bao and Bo Zhang and Chen Li and Zhenghua Li},
  journal={arXiv preprint arXiv:2206.11569},
  year={2022}
}
```

## Introduction
Some grammatical error correction (GEC) systems incorporate hand-crafted rules and achieve positive results. However, manually defining rules is time-consuming and laborious. In view of this, we propose a method to automatically mine error templates for GEC. 

We have accumulated 1,119 error templates along with their corrective actions for Chinese GEC so far (`./templates/zh`), and open-source 500 of them at present. Each template conforms to the following form:

```
A
B
1/2/3
```

We use the regular expression `A.*B` to represent a error template, and `1/2/3` denote three corrective actions (delete the left/right/random part). For more details, please kindly refer to our paper.

### Requirements

Python >= 3.6

### Usage

```
chmod +x example.sh
./example.sh
```

Expected output:

```
Fix 3 errors from 3 sentences.
```

## Contact
If you have any problems, feel free to raise an issue or contact [hillzhang1999@qq.com](mailto:hillzhang1999@qq.com).
