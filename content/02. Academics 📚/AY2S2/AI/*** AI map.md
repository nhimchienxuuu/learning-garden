---
mindmap-plugin: basic
time: 
tags:
---
# title
## Chapter 1: Introduction
- [[the importance of AI]]
- [[what is AI]]
- [[the different approached to AI]]

## Chapter 2: Intelligent Agents
- [[definition of an agent]]
- [[the structure of agents]]
- [[learning agents]]
---
## Lecture 2: Agents and Search
- [[options to design an AI agent]]
- [[designing rational agents]]
	- [[reflex agent]]
	- [[planning agent]]
- [[search problems]]
- [[state space]]
- [[state space graph vs search tree]]
	- [[state space graph]]
	- [[search tree]]
- [[search algorithm]]
	- [[tree search algorithm]]
	- [[depth-first search - dfs]]
	- [[breadth-first search - bfs]]
	- [[iterative deepening]]
	- [[cost-sensitive search]]
	- [[uniform cost search - ucs]]


## Lecture 3: Informed Search
- search so far
	- [[search problems]]
	- [[search tree]]
	- [[search algorithm]]
- [[pancake problem]]
- [[fringe strategy - the one queue]]
- [[uniform cost search - ucs]]
- [[search heuristics]]
- [[greedy search]]
- [[a* search]]
	- [[Optimality of A* Tree Search]]
	- [[properties of A*]]
	- A* applications
	- tree search, graph search notices
	- consistency of heuristics
	- optimality of A* graph search & summary
- [[admissible heuristics & creating admissible heuristics]]
	- example: 8 Puzzle I, II, III
- [[UCS vs A* Contours]]
- [[semi lattice of heuristics]]
	- trivial heuristics, dominance
- search models & search gone wrong


---
## [Search Heuristics](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C4%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Search%20Heu...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A19%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Search%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)[5](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C4%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Search%20Heu...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A19%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Search%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)

- **Heuristic Function**: Estimates how close a state is to a goal, designed for specific search problems.
- **Examples**: Manhattan distance, Euclidean distance for pathing.

## Greedy Search

- [**Strategy**: Expands the node that appears closest to a goal state based on a heuristic estimate](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C5%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20Strategy...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A28%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22%E2%97%8F%20Strategy%3A%20expand%20a%20node%20that%20you%20think%20is%20%5Cr%5Cnclosest%20to%20a%20goal%20state%22%2C%22snippets%22%3A%5B%5D%7D%7D)[6](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C5%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20Strategy...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A28%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22%E2%97%8F%20Strategy%3A%20expand%20a%20node%20that%20you%20think%20is%20%5Cr%5Cnclosest%20to%20a%20goal%20state%22%2C%22snippets%22%3A%5B%5D%7D%7D).

## A* Search

- **Combining UCS and Greedy**: Orders by the sum of backward cost ( g(n) ) and forward cost ( h(n) ).
- __Optimality of A_ Tree Search_*: Assumes admissible heuristics and claims that optimal goals will exit the fringe first.
- [**Properties of A***: Expands mainly toward the goal while ensuring optimality](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C6%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20A*%20expan...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A50%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A5%2C%22highlightText%22%3A%22%E2%97%8F%20A*%20expands%20mainly%20toward%20the%20goal%2C%20%5Cr%5Cnbut%20does%20hedge%20its%20bets%20to%20ensure%22%2C%22snippets%22%3A%5B%5D%7D%7D)[7](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C6%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20A*%20expan...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A50%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A5%2C%22highlightText%22%3A%22%E2%97%8F%20A*%20expands%20mainly%20toward%20the%20goal%2C%20%5Cr%5Cnbut%20does%20hedge%20its%20bets%20to%20ensure%22%2C%22snippets%22%3A%5B%5D%7D%7D).
- __A_ Applications_*: Used in various fields like video games, routing problems, and language analysis.
- **Tree Search and Graph Search Notices**: Importance of detecting repeated states and implementing a closed set.
- **Consistency of Heuristics**: Ensures estimated heuristic costs are less than or equal to actual costs.
- [__Optimality of A_ Graph Search & Summary_*: A* is optimal with admissible/consistent heuristics, and heuristic design is crucial](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C7%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20A*%20is%20op...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A74%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A3%2C%22highlightText%22%3A%22%E2%97%8F%20A*%20is%20optimal%20with%20admissible%20%2F%20consistent%20heuristics%5Cr%5Cn%E2%97%8F%20Heuristic%20design%20is%20key%3A%20often%20use%20relaxed%20problems%5Cr%5Cn74%22%2C%22snippets%22%3A%5B%5D%7D%7D)[8](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C7%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22%E2%97%8F%20A*%20is%20op...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A74%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A3%2C%22highlightText%22%3A%22%E2%97%8F%20A*%20is%20optimal%20with%20admissible%20%2F%20consistent%20heuristics%5Cr%5Cn%E2%97%8F%20Heuristic%20design%20is%20key%3A%20often%20use%20relaxed%20problems%5Cr%5Cn74%22%2C%22snippets%22%3A%5B%5D%7D%7D).

## [Admissible Heuristics & Creating Admissible Heuristics](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C8%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Creating%20A...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A55%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Creating%20Admissible%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)[9](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C8%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Creating%20A...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A55%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Creating%20Admissible%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)

- **Admissibility**: Heuristics must be optimistic and never outweigh true costs.
- **Example - 8 Puzzle**: Different heuristics like the number of tiles misplaced and total Manhattan distance.

## [UCS vs A* Contours](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C9%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22UCS%20vs%20A*%20...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A50%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22UCS%20vs%20A*%20Contours%22%2C%22snippets%22%3A%5B%5D%7D%7D)[10](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C9%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22UCS%20vs%20A*%20...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A50%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22UCS%20vs%20A*%20Contours%22%2C%22snippets%22%3A%5B%5D%7D%7D)

- **Comparison**: UCS expands equally in all directions, while A* focuses mainly toward the goal.

## [Semi Lattice of Heuristics](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C10%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Semi-Latti...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A63%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Semi-Lattice%20of%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)[11](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C10%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Semi-Latti...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A63%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Semi-Lattice%20of%20Heuristics%22%2C%22snippets%22%3A%5B%5D%7D%7D)

- [**Trivial Heuristics and Dominance**: The concept of dominance and the semi-lattice structure of heuristics](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C11%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Trivial%20He...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A64%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Trivial%20Heuristics%2C%20Dominance%22%2C%22snippets%22%3A%5B%5D%7D%7D)[12](https://edgeservices.bing.com/edgesvc/chat?udsframed=1&form=SHORUN&clientscopes=chat,noheader,udsedgeshop,channelstable,ntpquery,devtoolsapi,udsdlpconsent,udsmrefresh,cspgrd,&shellsig=b7539a3f524e16540d5348577f603192b931a009&setlang=en-US&darkschemeovr=1#sjevt%7CDiscover.Chat.SydneyClickPageCitation%7Cadpclick%7C11%7C8605d66a-4cd3-4298-8638-9cc159c5998c%7C%7B%22sourceAttributions%22%3A%7B%22providerDisplayName%22%3A%22Trivial%20He...%22%2C%22pageType%22%3A%22pdf%22%2C%22pageIndex%22%3A64%2C%22relatedPageUrl%22%3A%22file%253A%252F%252F%252FUsers%252Fchanity%252FDocuments%252FStudy%252FVINUNI%252FAY2-S2%252FAI%252FCOMP2050-Lecture%2525203-Informed-Search.pdf%22%2C%22lineIndex%22%3A1%2C%22highlightText%22%3A%22Trivial%20Heuristics%2C%20Dominance%22%2C%22snippets%22%3A%5B%5D%7D%7D).

## Search Models & Search Gone Wrong

- **Search and Models**: The effectiveness of search is dependent on the accuracy of the world models.
- **Search Gone Wrong**: Issues that arise when models do not accurately represent the real world.