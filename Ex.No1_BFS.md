# Ex.No: 1  Implementation of Breadth First Search 
### DATE:07/03/2025                                                                            

### REGISTER NUMBER : 212222220028
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1]To write a python program to implement Breadth first Search.

2]Call the bfs function by passing arguments visited, graph and starting node.

3]Stop the program.
### Program:
```
#breadth first Search in python 
graph = {
 '5' : ['3','7'],
 '3' : ['2', '4'],
 '7' : ['8'],
 '2' : [],
 '4' : ['8'],
 '8' : []
 }
 visited = [] # List for visited nodes.
 queue = []     #Initialize a queue
 def bfs(visited, graph, node): #function for BFS
 	 visited.append(node)
  	queue.append(node)
  		while queue:          # Creating loop to visit each node
    			m = queue.pop(0) 
    			print (m) 
    			for neighbour in graph[m]:
      				if neighbour not in visited:
        					visited.append(neighbour)
       					 queue.append(neighbour)

# Driver Code
print("Following is the Breadth-First Search")
bfs(visited, graph, '5')    # function calling
```
### Output:

![Screenshot 2025-03-07 151607](https://github.com/user-attachments/assets/1514c0ed-b271-4ef1-9025-7b2c2d71294d)


### Result:
Thus the breadth first search order was found sucessfully.
