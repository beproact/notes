We can call the node that represents your house $$h$$. We can call the node that represent your friend $$f$$.

We will assign two weights to every single node. One where we have already used the free toll, and one where we haven't. We can call these weighs $$W$$ for when the free toll hasn't been used and $$W'$$ for the free toll has been used. We puts these weights along with their nodes into priority queues $$Q$$ and $$Q'$$ for $$W$$ and $$W'$$ respectively.

We will define update as taking a node's weight and a value and changing the weight to value if value is less than the nodes weight.

Give every node a $$W$$ and $$W'$$ of $$\infty$$.  Give $$h$$ a $$W$$ and $$W'$$ of 0. 
Repeat this until $$Q$$ and $$Q'$$ are empty. Check which one has a least value at the top. If there's a tie, act as if $$Q$$ has the least value on top. 
If $$Q$$ has the least value, which we can call $$n$$, loop through every outgoing edge $$e = (n,v)$$. For each $$e$$ update $$W[v]$$ with the weight of n added to the edge weight and update $$W'[v]$$ with the weight of $$n$$. We then pop $$n$$ off the priority queue.
If $$Q'$$ had the least value, which we can call $$n'$$,  loop through each outgoing edge and update each receiving node with the weight of n added to the edge weight. We then pop $$n'$$ off the priority queue.

The cheapest route is the weight $$W'[f]$$. We can find the path by using the back pointers from the cheapest route.











The value in $$W$$ are updated exactly like how they are updated in Dijkstra's so we know that when we pop a node off of $$Q$$ it has the shortest path that involves no free tolls.  
The values in $$W'$$ are shortest paths when a free toll was used. This means that somewhere previously a free toll was used.  This effectively means that the path starts in a a graph where 




This algorithm is very similar to dijkstra's and has a runtime of $$O((|E|+|V|)\log|V|)$$.
This is because we have to do work for each edge and vertex. Each time we do that work we update the heap. Since the heap will have max of |V| items it takes, log|V| to update. This makes the runtime $$O(|E|+|V|) \cdot O(\log|V|)$$ or just $$O((|E|+|V|)\log|V|)$$.