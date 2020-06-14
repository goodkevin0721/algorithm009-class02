学习笔记

搜索
每个节点都访问一次
每个节点仅仅访问一次

深度优先（DFS）Depth-First-Search

递归:
visited = set()

def dfs(node,visited):
	if node in visited:
		return
	visited.add(node)
	
	for next_node in node.children();
		if not next_node in visited
			dfs(next_node,visited)

非递归
def DFS(self,tree)
	if tree.root is None
		return []
	visited, stack = [],[tree.root]
	while stack:
		note = stack.pop()
		visited.add(node)
		
		process(node)
		nodes = generate_related_nodes(node)
		stack.push(nodes)
		
广度优先（BFS） Breadth-First-Search


def BFS(graph,start,end)
	queue = []
	queue.append([start])
	visited.add(start);
	
	while queue:
		node = queue.pop();
		visited.add(node)
		
		process(node)
		nodes = generate_related_nodes(node)
		queue.push(nodes)
	
贪心算法：每一步选择中都采取在当前状态最好或最优的选择，从而导致结果是全局最好或最优的算法
贪心算法：
每个子问题都作出选择，不能回退
动态规划：
保存以前的运算结果，并根据以前的结果对当前进行选择，有回退功能

二分查找
1.单调递增递减
2.存在上下界
3.通过索引访问

left，right = 0,len(array)-1
while left < right
	min = left + right;
	if array[mid] == target
		break or return result
	elif array[mid] < target
		left = mid + 1
	else
		right = mid - 1

