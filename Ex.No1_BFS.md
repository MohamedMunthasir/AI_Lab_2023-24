# Ex.No: 1  Implementation of Breadth First Search 
### DATE:                                                                            
### REGISTER NUMBER : 212222220025
### AIM: 
To write a python program to implement Breadth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function bfs and take the set “visited” is empty and “queue” is empty
4. Search start with initial node and add the node to visited and queue.
5. For each neighbor node, check node is not in visited then add node to visited and queue list.
6.  Creating loop to print the visited node.
7.   Call the bfs function by passing arguments visited, graph and starting node.
8.   Stop the program.
### Program:
```
graph = {
    '5': ['3', '7'],
    '3': ['2', '4'],
    '7': ['8'],
    '2': [],
    '4': ['8'],
    '8': []
}

def bfs(graph, node):
    visited = []  # List for visited nodes.
    queue = []    # Initialize a queue

    visited.append(node)
    queue.append(node)

    print("Following is the Breadth-First Search:")

    while queue:
        m = queue.pop(0)
        print(m, end=" ")  # Print the node
        
        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

# Driver Code
bfs(graph, '5')
```
### Output:
![WhatsApp Image 2025-06-01 at 14 46 07_ba6a7cdf](https://github.com/user-attachments/assets/63f3aa76-e23a-47cd-845e-1a9e72317557)



### Result:
Thus the breadth first search order was found sucessfully.
