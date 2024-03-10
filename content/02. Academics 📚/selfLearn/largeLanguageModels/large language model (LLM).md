---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
## description
- it is pre trained answers data that is used to respond your questions
- include 2 files (parameters & a C code file of running those parameters)
- eg. llama2-70b
	- released by meta ai
	- 2: 2nd version
	- 70b: 70 billion parameters; other models include 7, 13, 34
	- liked by many as the world most powerful open-weights model (gpt model architecture is not released, it is owned by open AI, can only use through a web chatgpt)
- every parameter is stored as 2 bytes -> 70bil parameter = 140 GB
	- 2 bytes: float 16 number #toExplore 
- parameter running file
	- can be C, Python, or any
	- not a lot storage needed to run -> the question in how to get the parameter, what is it

## LLM training
- neural network - predict the next word in the sequence
	- ![](https://i.imgur.com/2ifp84d.png)
	- close relationship btw prediction and compression
	- being forced to learn a lot about the world to work