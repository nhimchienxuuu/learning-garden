---
mindmap-plugin: basic
time: 2023-12-25T14:30:00
tags: 
source:
---
# Unsupervised Learning
- Unsupervised learning
	- Training LLMs like GPT-4
		- considered as UL, or commonly as self-supervised learning (subset of UL)
		- dont have explicit labels or target outputs, but rather learning to predict next word in a sentence, given the previous words
		- using the input text itself as both input and output
	- data: given input x, but not output labels y
		- eg. data on patients, tumor's size, patient's age
	- goal: find sth interesting / patterns / structure in unlabeled data, not whether benign or malignant 
	- clustering algo:
		- [visualization](https://www.ejable.com/wp-content/uploads/2023/11/Unlabeled-data-vs.-labeled-clusters-2.webp)
		- place data in different clusters
		- eg. gg news, group related stories together by keywords, in which the algo figure out by itself without supervision
	- will also learn
		- anomaly detection: find unusual data points
		- dimensionality reduction: compress data using fewer numbers
<!--ID: 1708098044311-->
