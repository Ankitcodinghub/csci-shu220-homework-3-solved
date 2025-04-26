# csci-shu220-homework-3-solved
**TO GET THIS SOLUTION VISIT:** [CSCI-SHU220 Homework 3 Solved](https://www.ankitcodinghub.com/product/csci-shu220-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;133189&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI-SHU220 Homework 3  Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
This assignment has in total 55 base points and 10 extra points, and the cap is 55. Bonus questions are indicated using the ⋆ mark.

Please specify the following information before submission:

• Your Name: Yufeng Xu

• Your NetID: yx3038

Problem 1: Infinite knapsack [10⋆ +15 pts]

(a)⋆ Prove that in any optimal solution (n1,…,nm), the total number of copies of the items I2,…,Im included in the knapsack is at most wmax − 1, i.e.,

(b) Based on the conclusion of (a), design an algorithm Knapsack(m,W,(w1,v1),…,(wm,vm)) for infinite knapsack with running time ). For convenience, your algorithm only need to return the maximum value achieved. Describe the basic idea and give the pseudocode. Briefly justify the correctness and analyze the time complexity.

(Hint: According to (a), we know that, in an optimal solution, the total weight of the items

), and hence the item I1 occupies “most” space of the knapsack. Try to

combine this observation with the O(mW)-time DP algorithm.)

Solution. Please write down your solution to Problem 1 here.

(a) We prove the problem by contradiction. Suppose there exists an optimal solution where

. We denote these items as where n ≥ wmax, and for each ,

∃i = 2,…,m such that wj′ = wi. There can be multiple wj′ s that are equal to the same wi.

Now, we want to show that ∃1 ≤ l ≤ r ≤ n such that is a multiple of w1. Consider the sum of the first k wj′ s, denoted as . Assume Sk ≡ Rk(mod w1), where Rk = 0,1,…,w1−1. (i) if ∃k such that Rk = 0, then take is a multiple of w1. (ii) if ∄k such that Rk = 0, Rk can only take w1 − 1 possible values. Because n ≥ wmax ≥ w1 ≥ w1 − 1, by the Pigeon-hole Principle, ∃k1,k2 such that Rk1 = Rk2, hence take w1).

Next, we can take 1 ≤ l ≤ r ≤ n such that

. Therefore, we can replace with t w1’s, and the final

value is going to be larger, which is contradictory to our assumption that the original solution is optimal.

Therefore, , i.e.,

(b) We know from (a) that 1, hence .

Consider the naive infinite knapsack algorithm. Let DP(i,w) represent the maximul value by choosing from items {i,i + 1,…,m} with total weight w. Because we can either take ni the i-th item or take none of them, DP(i,w)=max{DP(i + 1,w), vi+DP(i,w − wi)}. Because i = 1,2,…,m, w = 0,1,…,W, hence this algorithm is of time complexity O(nW).

Now, with the conclusion from (a), we can limit the search space of w for i = 2,…,m to . Then, the global maximum is equal to maxw{DP(2,w .

For items 2,…,m, given any total weight limit w, with the infinte knapsack problem, we can obtain the optimal solution that maximizes the total value of the items chosen. For the whole problem, we learned from (a) that the total weight of items 2,…,m ≤ wmax2. Therefore, we can limit the total for 2,…,m to wmax2 and simply take as many item 1 as possible for the weight limit we haven’t used. By using this method, we can obtain the correct optimal solution.

Because the weight limit for item 2,…,m shrinks from , and it takes O(1) time to add item 1 to the partial solution, the time complexity of the revised algorithm is

Below is the pseudocode:

def KNAPSACK(m, W, I ):

# I is a l i s t of (w, v ) ’ s

I = sorted(I , key=lambda x : x . v / x .w) w max = max([ item .w for item in I ])

DP = [[0 for w in range(w max ∗∗ 2)] for idx in range(m + 1)]

# m+1 is set to handle boundary cases for idx in range(m − 1 , 0 , −1):

for w in range(w max ∗∗ 2 + 1):

if w &gt;= I [ idx ] .w:

DP[ idx ] [w] = max( I [ idx ] . v + DP[ idx ] [w − I [ idx ] .w] , DP[ idx + 1][w]) else :

DP[ idx ] [w] = DP[ idx + 1][w]

ans = max([DP[ 1 ] [w] + floor ((W − w) / I [ 0 ] .w) ∗ I [ 0 ] . v ]) return ans

Problem 2: Counting shortest paths [15 pts]

Given an undirected graph G = (V,E) and a vertex s ∈ V , we want to know for every vertex t ∈ V , how many (distinct) shortest paths from s to t there are. This can be viewed as a generalization of the unique shortest-path problem. Design an algorithm Count(G,s) to solve this problem. The algorithm should return a list L that contains a pair (v,δv) for each vertex v of G, where δv is the number of shortest paths from s to v. Describe the basic idea and give the pseudocode. Briefly justify the correctness and analyze the time complexity. Your algorithm should run in O(n + m) time, where n = |V | and m = |E|.

A sample example. Suppose the input graph is G = (V,E) where V = {s,a,b,c,d,e} and

E = {(a,b),(b,c),(c,d),(a,d),(s,a),(c,e)}; see the figure below. Then the algorithm Count(G,s) should return L = [(s,1),(a,1),(b,1),(c,2),(d,1),(e,2)].

(Hint: Exploit the BFS tree and extend the idea in the unique shortest-path problem.)

Solution. Please write down your solution to Problem 2 here.

We solve the problem by BFS. Consider a BFS tree of the graph, we view s as the root, and perform a level-order traversal. For each node, we count the number of it on that level as the number of shortest paths. For the neighbors of that node, if the number of shortest paths has not been counted for a neighbor, we append it to the queue that maintains the BFS tree, otherwise we just ignore it, because it must have been studied in a higher level, and the node’s appearance in the current level does not corresponds to a shortest path.

The pseudocode is as follows:

class Node:

def i n i t ( s e l f ):

s e l f . neighbors = [ ]

def add neighbor ( self , other ): s e l f . neighbors . append( other ) other . neighbors . append( s e l f )

def COUNT(G, s ):

(V, E) = G

# V: l i s t of Node ; E: l i s t of tuples of 2 Nodes for edge in E:

edge [ 0 ] . add neighbor ( edge [1])

cnt = {} queue = [ s ] while queue != [ ] : L = len(queue) print(L) for u in queue [ : L ] : cnt [u] = cnt . get (u, 0) + 1 print(u. neighbors ) for v in u. neighbors :

if v not in cnt . keys ():

queue . append(v)

queue = queue [L : ]

L = [( item [0] , item [1]) for item in cnt . items ()] return L

This algorithm is correct because all the nodes that have the same shortest-path-length are on the same level of the BFS tree, so by counting the times a node appear in the shallowest level where it appears, we can count the number of shortest paths to the node.

Because only the shortest path will be considered, each edge will be visited once and only once. The sum of the number of times each node is visited is O(m), therefore, this algorithm is O(m) (and consequently O(m + n)).

Problem 3: Reaching the one [15 pts]

Let n ≥ 3 be a given positive integer and we are going to play a game as follows. During the game, we have a number k which is initially equal to 2. In each round of the game, we are allowed to change the current number k to a new number in one of the following ways:

• Type-A: Change k to (k + 1) mod n.

• Type-B: Change k to a divisor of k that is greater than 1.

• Type-C: Change k to k2 mod n.

Note that the above three rules guarantee that our number k is always in the range {0,1,…,n−1} during the entire game. The game terminates when k becomes 1. Our goal is to finish the game in fewest rounds. For example, suppose n = 91 and we can play the game as follows.

• Round 1: 2 =⇒ 3 using Type-A change. • Round 2: 3 =⇒ 9 using Type-C change.

• Round 3: 9 =⇒ 81 using Type-C change.

• Round 4: 81 =⇒ 27 using Type-B change.

• Round 5: 27 =⇒ 1 using Type-C change.

As you can verify, this is an optimal solution. Design an algorithm Game(n) which returns an optimal solution to the game as a list. So Game(91) should return [2,3,9,81,27,1] (or another solution with 5 rounds). Describe the basic idea and give the pseudocode. Briefly justify the correctness and analyze the time complexity. Your algorithm should run in O(nlogn) time.

(Hint: Formulate the problem as a graph problem with n vertices and O(nlogn) edges.)

Solution. Please write down your solution to Problem 3 here.

We construct a graph based on the problem setting: all the possible remainders of n: 0,1,…,n−1 are constructed as n vertices.

For Type-A operation, we connect vertex k to vertex k+1 for k = 0,1,…,n−2, and connect n−1 to 0.

For Type-B operation, we connect vertex k to all its divisors larger than 1.

For Type-C operation, we connect vertex k to k2(mod n) for k = 2,…,n − 1.

Next, we consider the total number of directed edges. For Type-A, the number of directed edges is n; for Type-B, the total number of edges is ; for Type-C, the total number of edges is n − 2.

Therefore, the total number of directed edges

1) . By integral test, +1, where ). Therefore, )). Also, n is O(nlog(n)), hence the number of directed edges is O(nlog(n)).

Next, we perform a BFS search on this graph G. We use a queue to maintain the BFS procedure. We first append the starting vertex 2 to the queue. Every time, for the first vertex in the queue, if it’s 1, we quit the BFS; otherwise we append all of its unvisited neighbors to the end of the queue, and mark the current vertex the previous vertex of all its neighbors (if a neighbor does not have a recorded previous vertex).

This algorithm can always find the shortest path between 2 and 1, because the nearest vertex will always come to the head of the queue. So when 1 is visited, the path is guaranteed to be shortest.

The time complexity of BFS is O(nlog(n)) because the total number of edges in the graph is

O(nlog(n)), and each edge is visited at most once. The time needed to construct the graph is also O(nlog(n)) because each edge takes O(1) time to construct. Therefore, the overall complexity of the algorithm is O(nlog(n)).

The pseudocode is given as follows:

class Vertex :

def i n i t ( self , val ): s e l f . val = val s e l f . neighbors = [ ]

def add neighbor ( self , other ):

s e l f . neighbors . append( other )

def GAME(n ):

V = [ Vertex ( i ) for i in range(n )]

# Type A edge for i in range(n − 1):

V[ i ] . add neighbor (V[ i + 1])

# Type B edge for i in range(2 , n ):

for j in range(2 ∗ i , n, i ):

V[ j ] . add neighbor (V[ i ])

# Type C edge for i in range(2 , n ): if i ∗∗ 2 % n != i :

V[ i ] . add neighbor (V[ i ∗∗ 2 % n ])

# BFS visited = [0 for i in range(n )]

prev = [−1 for i in range(n )] queue = [2] while queue != [ ] : head = queue [0] queue = queue [ 1 : ] visited [ head ] = 1 if head == 1: break

for n in V[ head ] . neighbors :

if not visited [n. val ] : queue . append(n. val )

if prev [n. val ] == −1:

prev [n. val ] = head

sol = [1]

while sol [−1] != −1: sol . append( prev [ sol [ −1]])

return sol [ −2:: −1]

Problem 4: Finding a strongly connected component [10 pts]

Given a directed graph G = (V,E) and a vertex s ∈ V , we want to compute the strongly connected component of G containing s. Design an algorithm SCC(G,s) which returns the set of vertices of G that lie in the same strongly connected component as s. Describe the basic idea and give the pseudocode. Briefly justify the correctness and analyze the time complexity. Your algorithm should run in O(n + m) time, where n = |V | and m = |E|.

(Hint: By definition, a vertex v is in the same strongly connected component as s iff v is reachable from s and s is reachable from v. We already know how to find the vertices reachable from s using DFS. Can you use a similar idea to compute the vertices from which s is reachable?)

Solution. Please write down your solution to Problem 4 here.

For each node u, we store all the nodes v that (u,v) ∈ E as its out-neighbors and all the nodes w that (w,u) ∈ E as its in-neighbors. Then we perform DFS based on out-neighbors to obtain all the nodes that s can reach, and DFS based on in-neighbors to obtain all the nodes that can reach s. Lastly, we take the intersection of the two results, so that we can obtain the set of points in the strongly connected components containing s.

This algorithm is correct, as we know DFS can reach a point t iff it’s reachable from s. If we reverse the directions of all edges, and perform DFS again, a point t is reached iff ∃ a path consisting of reversed from s to t, i.e., ∃ a edge from t to s, s is reachable from t. By taking the union of the results obtained by the 2 DFS’s, a node t is kept iff it is reachable from s and it can reach s, i.e., it is strongly connected to s.

The time complexity to process in-neighbors and out-neighbors is O(m). The time complexity of DFS is O(n + m). Therefore, the time complexity of the whole algorithm is O(n + m).

The pseudocode is as follows:

class Node:

def i n i t ( self , val ): s e l f . val = val

s e l f . neighbors = [ [ ] , [ ] ] # 0 for in , 1 for out

def add neighbor ( self , other ):

s e l f . neighbors [ 1 ] . append( other ) other . neighbors [ 0 ] . append( s e l f )

# add a edge from s e l f to other

def SCC(G, s ):

(V, E) = G for (u, v) in E:

u. add neighbor (v)

res = [ set () , set ()]

# res [0] for a l l the nodes can be reached from s ; # res [1] for a l l the nodes that can reach s def DFS(u, direction = 0):

# direction = 0 for in−neighbors , 1 for out−neighbors res [ direction ] . add(u)

for v in u. neighbors [ direction ] :

if v not in res [ direction ] :

DFS(v , direction = direction )

DFS(s , 0)

DFS(s , 1) ans = res [ 0 ] . intersection ( res [1])

ans . remove( s ) return ans
