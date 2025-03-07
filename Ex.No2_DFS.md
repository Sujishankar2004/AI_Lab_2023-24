# Ex.No: 2  Implementation of Depth First Search
### DATE:                                                                            

### REGISTER NUMBER : 212222220028
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1.To write a python program to implement Depth first Search.
2. Call the dfs function by passing arguments visited, graph and starting node.
3. Stop the program.
### Program:
```
graph = {
  '5' : ['3','7'],
  '3' : ['2', '4'],
  '7' : ['8'],
  '2' : [],
  '4' : ['8'],
  '8' : []
}
visited = set() # Set to keep track of visited nodes of graph.
def dfs(visited, graph, node):  #function for dfs 
    if node not in visited:
        	print (node)
        	visited.add(node)
        	for neighbour in graph[node]:
            	dfs(visited, graph, neighbour)
# Driver Code
print("Following is the Depth-First Search")
dfs(visited, graph, '5')
```
### Output:

![Screenshot 2025-03-07 151558](https://github.com/user-attachments/assets/55d51173-2d95-4587-9601-9dcb677b4059)


### Result:
