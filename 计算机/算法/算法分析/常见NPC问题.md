图问题
  图遍历问题分类（其中第一种不是NPC问题）：
		遍历所有边不重复 = 欧拉路径/一笔画问题
		遍历所有点不重复 = 哈密顿回路问题
		遍历所有边可以重复 = 中国邮递员问题（对无向图为P问题，对有向图为NPC问题）
		遍历所有点可以重复 = 旅行商问题（TSP）
	图着色问题：对一个无向图染色，满足相连点的颜色都不同，问最少需要多少种颜色
	分团问题：问一个图中是否存在顶点个数为k以上的clique（一个子图，满足其中的顶点两两相连）
	最小覆盖（虽然包括顶点覆盖和边覆盖，但实际只指顶点覆盖，只有顶点覆盖为NPC问题）：
		对图G，其中每个顶点均可覆盖所有以它为顶点的边，问最少选多少个点可覆盖所有的边
	独立集
	子图同构问题（注意图的同构问题目前还未被证明为NP问题）
	
		
	
数学问题：
	背包问题——最优化描述：
		对于给定容量的背包和给定价值以及大小的很多物品，问如何选择能使背包装的总价值最高
	背包问题——确定性描述：
		对于给定容量的背包和给定价值以及大小的很多物品，问能否选出物品总价值不超过V（在不超过背包容量的前提下）
	子集和问题：
		给定一个整数集合，问是否存在子集，使其和为k
	
	
其它问题：
	扫雷
	华容道问题/(n^2-1)数码问题
	布尔可满足性质问题
