# JointPS: [A Simple and Effective Neural Model for Joint Word Segmentation and POS Tagging](https://zhangmeishan.github.io/ChineseLexicalProcessing.pdf)
Joint models have shown stronger capabilities for Chinese word segmentation and POS tagging, and have received
great interests in the community of Chinese natural language processing (NLP). In this paper, we follow this line of work, presenting a simple yet effective sequence-to-sequence neural model for the joint task, based on a well-defined transition system, by using long short term memory (LSTM) neural network structures. We conduct experiments on five different datasets. The results demonstrate that our proposed model is highly competitive. By using well-trained character-level embeddings, the proposed neural joint model is able to obtain the best reported performances in the literature.


# Requirement:
	Python  == 3  
	PyTorch == 0.3.1

# Usage  
	modify the config file, detail see the Config directory
	Train:
	(1) sh run_train_p.sh
	(2) python -u main.py --config ./Config/config.cfg --train -p 

# Config


# Network Structure
![](https://i.imgur.com/wIAMutu.png)

# Performance


|  | CTB5 | CTB6 | CTB7 | PKU | NCC |   
| :----------: | ---------- | ---------- | ---------- | ---------- | ---------- |     
| **Model** | **SEG**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**POS** | **SEG**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**POS** | **SEG**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**POS** | **SEG**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**POS** |  **SEG**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**POS** |  
| Our Model (No External Embeddings)  | 97.69&nbsp;&nbsp;&nbsp;&nbsp;94.16 | 95.37&nbsp;&nbsp;&nbsp;&nbsp;90.83 | 95.32&nbsp;&nbsp;&nbsp;&nbsp;90.25 | 95.22&nbsp;&nbsp;&nbsp;&nbsp;92.62 | 93.97&nbsp;&nbsp;&nbsp;&nbsp;89.47 |     
| Pipeline (No External Embeddings)  | 97.15&nbsp;&nbsp;&nbsp;&nbsp;93.72 | 94.85&nbsp;&nbsp;&nbsp;&nbsp;90.08 | 94.71&nbsp;&nbsp;&nbsp;&nbsp;89.56 | 94.86&nbsp;&nbsp;&nbsp;&nbsp;91.84 | 93.54&nbsp;&nbsp;&nbsp;&nbsp;88.52 |    
| Our Model (Basic Embeddings)  | 97.93&nbsp;&nbsp;&nbsp;&nbsp;94.44 | 95.78&nbsp;&nbsp;&nbsp;&nbsp;91.79 | 95.77&nbsp;&nbsp;&nbsp;&nbsp;91.12 | 95.82&nbsp;&nbsp;&nbsp;&nbsp;93.42 | 94.52&nbsp;&nbsp;&nbsp;&nbsp;89.82 |      



# Cite
	@Article{zhang2018jointposseg,  
	  author    = {Zhang, Meishan and Yu, Nan and Fu, Guohong},  
	  title     = {A Simple and Effective Neural Model for Joint Word Segmentation and POS Tagging},  
	  journal   = {IEEE/ACM Transactions on Audio, Speech and Language Processing (TASLP)},  
	  year      = {2018},  
	  volume    = {26},  
	  number    = {9},
	  pages     = {1528--1538},
	  publisher = {IEEE Press},
	}

# Schedule
updating.