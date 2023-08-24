# Algebraic Graph Theorem

## Part1: Linear algebra in graph theory

### Section2: The spectrum of a graph

- **Definitions**:
    
    - *spectrum.*
        
    - 特征多项式：
        
    
    - Two non-isomorphic graphs are said to be *cospectral* if they have the same eigenvalues with the same multiplicities.
        
- * * *
    
- **Proposition**:
    
    - $c_1 =0$, $-c_2=e(G)$, $-c_3=$2\*#number of triangles in G.
        
    - Lemma2.5: Then number of walks of length $l$ in G, from $v_i$ to $v_j$ is the entry of $A^l(i,j)$.
        
    - Prop2.6: A(G)’s dimension is at least $diam(G)+1$.
        
    - Results 2c: The spectrum of a bipartite graph is symmetric with respect to 0.
        
- * * *
    
- **Words**:
    

> principal minor: 主子式

* * *

### Section3: Regular graphs and line graphs

- **Definitions:**
    
    - $J$: the matrix each of those entries is $+1$.
        
    - $\mathscr{A}(G)$ : G 的邻接矩阵的多项式矩阵。
        
    - $P(A)$ : the minimum polynomial; $p(\lambda)=(\lambda-k)q(\lambda)$; $q(A) = \alpha J$
        
    - Circulant graph: a graph whose vertices can be ordered so that the adjacency matrix of $G$ is a circulant matrix. $a_1=1, a_i = a_{n-i+2}$.
        
    - $A_L$: the adjacency matrix of $L(T)$.
        
- * * *
    
    ### Proposition:
    
    - Let G be a k-regular graph, then:
        
        1): k is and eigenvalue of G;
        
        2):if G is connected, the multiplicity of k is 1;
        
        3): for any eigenvalue $\lambda$ of G, $|\lambda|\leq k$.
        
    - The matrix $J$ belongs to the adjacency algebra $\mathscr{A}(G)$ if and only if $G$ is a regular connected graph.
        
    - eigenvalues of G: $\lambda_r = \sum_{j=2}^na_j\omega^{(j-1)r}$.
        
    - The  eigenvalues of a line graph is $\geq -2$
        
- * * *
    
- **words**:
    
    > adjacency algebra: 临接代数
    

* * *

### Section 4:Cycles and cuts

- ### Definitions:
    
    - vertex-space $C_o(G)$ : vector space of all functions from $V(G)$ to $\mathbb{C}$
        
    - edge-space $C_1(G)$ : vector space of all functions from $E(G)$ to $\mathbb{C}$
        
    - incidence mapping: for each $\xi$ : $E(G) \to \mathbb{C}$, the function $D\xi:V(G)\to \mathbb{C}$ is defined:
        
        $D\xi (v_i)=\sum_{j=1}^md_{ij}\xi(e_j)$.( $d_{ij}$ is respect to the directed graph).
        
    - rank of $G$ : $r(G) = n-c$;(is the rank of incident matrix $T$).
        
    - co-rank of $G$: $s(G)=m-n+c$(is the dimension of the kernel of incidence mapping $D$ of $T$ .
        
    - inner-product: $(\rho,\sigma)=\sum_{\in ET}\rho(e)\overline{\sigma(e)}$.
        
- * * *
    
- **Proposition:**
    
    - The incidence matrix D of G has rank $n-c$. $c$ is the number of components.
        

* * *

### Section 5: Spanning trees and associated structures

## Key Lemma:

    Let $T$ be the spanning tree in a connected graph $G$.Then:

    1) for each edge $g$ of $G$ which is not in $T$, there is a unique cycle in $G$ containing $g$ and edges in $T$ only.

    2) fir each edge $h$ of $G$ which is in $T$, there is a unique cut in $G$ containing $h$ and edges not in $G$ only.

## Definitions:

- $cyc(T,g)$ and $cut(T,h)$ : the unique cycle and cut defined above.
    

## Propositions:

- $T$ be a spanning tree of $G$ and let $a$ and $b$ be edges of $G$ such that $a\in G$ and $b\notin G$. Then
    
    $b\in cut(T,a) == a \in cyc(T,b)$.
    

* * *

# Section 6: Tree number

## Definitions:

- $\kappa(G)$: the number of spanning trees of a graph $G$, is the tree number.
    
- $\sigma(G;\mu) = det(\mu I-Q)$.
    

## Propositions:

- $Q=DD^t$, then the $adj Q$ is a multiple of $J$. $adj Q = \kappa (G) J$.
    
- $\kappa(G) = n^{-2}det(J+Q)$.
    

- If G is a regular graph with degree k, then :
    
    $\kappa(L(G))=2^{m-n+1}k^{m-n}\kappa(G)$.
    
- 可以得到关于完全多部图$K_{a_1,\dots,a_s}$ 的 tree number.
    
    $\kappa(K_{a_1,\dots,a_s})= n^{s-2}(n-a_1)^{a_1-1}\dots (n-a_s)^{a_s-1}$.
    

# Section 7: Determinant expansions

## Definitions:

- elementary graph: a simple graph , each component is a single edge ($K_2$) or a cycle.
    
- $p(\Phi)$:  the product of the numbers of vertices in the components of $\Phi$,
    

## Propositions:

- Let $A$ be the adjacency matrix of a graph $G$. Then
    
    $det A=\sum(-1)^{r(\Lambda)}2^{s(\Lambda)}$, where the summation is over all spanning elementary subgraphs $\Lambda$ pf $G$.
    
- $(-1)^ic_i=\sum(-1)^{r(\Lambda)}2^{s(\Lambda)}$,where the summation is over all elementary subgraphs $\lambda$ of $G$ with $i$ vertices.
    
- $(-1)^iq_i = \sum p(\Phi)$, where the summations is over all sub-forests $\Phi$ of $G$ which have $i$ edges.
    

# Section 8: Vertex-partitions and the spectrum

## Definitions:

- Rayleigh quotient: $(z,Xz)/(z,z)=R(X;z)$.
    

## Propositions:

- $G$ is a bipartite graph and $\lambda$ is an eigenvalue of multiplicity $m(\lambda)$. Then $m(-\lambda)=m(\lambda)$.
    
- $\lambda_{max}(X)\geq R(X;z)\geq \lambda_{min}(X)$
    
- If $\lambda$ is an induced subgraph of $G$, then ,
    
    $\lambda_{max}(\Lambda)\leq\lambda_{max}(G)$; $\lambda_{min}(\Lambda)\geq \lambda_{min}(G)$
    
- $\Delta (G)\geq \lambda_{max}(G)\geq \delta_{ave}(G)\geq \delta(G)$
    
- （Wilf 1967) For any graph $G$ we have : $\chi(G)\leq 1+\lambda _{max}(G)$
    
- $\lambda_{max} (K_{a,b})=\sqrt{ab}$.
    
- (Hoffman) $\chi (G)\geq 1+\frac{\lambda_{max}(G)}{-\lambda_{min}(G)}$.
    

# Section 9: The chromatic polynomial

## Definitions:

## Propositions:

- $C(G;s)$ is  the number of vertex-colourings of $G$ using at most $s$ colours.
    
- $C(G;u) = C(G^{(e)};u)-C(G_{(e)};u)$
    
- If T is a tree with n vertices then: $C(T;u)=u(u-1)^{n-1}$.
    
- $C(C_n;u)=(u-1)^n+(-1)^n(u-1)$
    
- If $G=G_1+G_2$, then $m_i(G)=\sum_{j+l=i}m_j(G_1)m_l(G_2)$
    
- $C(G_1+G_2;u)=C(G_1;u)\circ C(G_2;u)$
    
- If the graph $G$ has quasi-separation $(V_1,V_2)$ then $C(G;u)=\frac{C(<V_1>;u)C<V_2>;u)}{C<V_1\cap V_2>;u)}$
    

# Section 10: Subgraph expansions

## Definitions:

- $\rho _{ij}$: The number of sungraph with rank i and co-rank j.
    

## Propositions:

- $C(G;u)=\sum_{w\in [u]^{VG}}\Pi_{e\in EG}w(e)$
    
- $C(G;U)=\sum_{S\subset EG}(-1)^{|S|}u^{n-rS}$

- $(-1)^i b_i$ is the number of subgraphs of $G$ which have $i$ edges and contain no broken cycles.
    
- $b_i=0$ for all $i=n,n-1,…,n-(c-1)$,(因为一个图的色多项式，等于其联通分支的色多项式的乘积）
    
- If $G$ is a strict graph with rank $r$.Then the coefficients of $C(G;u)$ alternate strictly in sign
    

# Section11: The multiplicative expansion

## Definitions:

- Let $X$ be the real-valued function defined by:
    
    $X(G)=\sum_{S\subset EG}Y(S)$.
    

## Propositions:

- If the functions $Y$ satisfies $P_1$ and $P_2$ ,then the corresponding function $X$ satisfies the same properties.
    
- $\sum_{I\subset J}(-1)^{|I|}=0$.
    
- Let $G$ be a general graph.If G has no edges ,or if $G$ is separable and has no isolated vertices, then $\widetilde{X}(G)=0$.
    

- we can prove $log X(G)=\sum_{S\subset EG}\widetilde{X}(S)$.
    

- $q(G,u)=\widetilde{Y_u}(G)$.（根据定义，在图$G$ 是separatable时，$\widetilde{Y_u}(G)=1$.
    

# Section12: The induced subgraph expansion

## Definitions:

- $Q(G;u)=\Pi q(\Gamma;u$), where the product is over the set of spanning sungraphs $\Gamma$ of $G$.
    

## Propositions:

- $C(G;u)=u^{|VG|}$$(1-u^{-1})^{|EG|}\Pi Q(G;u)$.
    

- If the graph $G$ is quasi-separable, then $Q(G;u)=1$
    
- The chromatic polynomial of a graph is determined bi its proper induced subgraphs whcih are not quasi-separabel.
    

# Section13: The Tutte polynomial

## Definitions:

- $T(G;x,y)=T(G^{(e)};x,y)+T(G_{(e)};x,y)$.
    
- $\lambda(X)$: The first edge which added in $X$ will increase $r(X)$ by $1$.
    
- $\mu(X)$: The first edge which deleted from $X$ will decrease $s(X)$ by $1$.
    
- An edge $e$ in $EG \setminus X$ is externally active with respect to $X$ if $\mu (X\cup e)=e$.
    
- An edge $e$ in $X$ is internally active with respect to $X$ if $\lambda (X\setminus e)=e$.
    

## Propositions:

([Biggs, p. 106](zotero://select/library/items/XMMWLXB6))

- If $A\subset B\subset A^\lambda$, then $B^\lambda = A^\lambda$.
    
- If $A\subset B$ and $r(B)\neq r_0$, then $\lambda(B) \in A^\lambda$.
    

- $r(X)=r_0$ and $X^\lambda=X$.Then $X=Y^\lambda == X^-\subset Y\subset X$.
    
- If $T$ is  a spanning tree, and suppose $W\in C$ such that $W^\lambda =T$. Then $W^\epsilon=T^\epsilon$
    
- The Tutte polynomial of a connected graph $G$ is independent of the ordering used in its definition.
    

# Section14: Chromatic polynomials and spanning trees.

## Definitions:

- $\theta(G)$: of a connected graph $G$ is the number of spanning tress of $G$ which have internal activity 1 and external activity 0.
    

## Propositions:

- Let $G$ be a connected graph with $n$ vertices. Then $C(G;u)=(-1)^{n-1}u\sum_{i=1}^{n-1}t_{i0}(1-u)^i$.
    
- $t_{10}=t_{01}$.
    
- If $G_1$ and $G_2$ are homeomorphic connected graphs with at least two edges, then $\theta(G_1)=\theta(G_2)$.( it fail in the graoh $K_2$.)
    
- $c_{i-1}\leq c_i$ for all $i\leq \frac{1}{2}(n-1)$.
    

# Section15: Automorphisms of graphs

## Definitions:

- $G$ is vertex-transitive: if for any $u,v$ there exist a $\pi\in Aut(G)$ such that $\pi(u)=v$.
    
- We can similarly define edge-transitive.
    

## Propositions:

- If a connected graph is edge-transitive but not vertex-transitive, then it is bipartite.
    
- $\pi$ is an automorphism of $G$ if and only if $PA=AP$, where $P$ is the permutation matrix representing $\pi$.
    

# Section16: Vertex-transitive graph

## Definitions:

- $G_v$: the subgroup of $G$ containing those automorphisms which fix $v$.
    

- If any  element of $G$ (except the identity) does not fix any vertex, we say it **regularly**.(只有唯一的同构映射$h_{ij}$ s.t. $h_{ij}(v_i)=v_j$.
    
- A group $G$ is graphical regular representation ,or GRR is there is a graph $\Gamma$ such that $G$ is isomorphic with $Aut(\Gamma)$ acts regularly on $V\Gamma$.
    

## Propositions:

- $|G|/|G_v|=|VG|$.
    
- Caley图是 vertex-transitive 的
    
- $\pi$ is an automorphism pf the group $G$ such that $\pi(\Omega)=\Omega$，then $\pi$ is a permutation of the vertices of $T(G,\Omega)$ is a graph automorphism fixing the vertex 1.
    

- If $Aut(\Gamma)$ is abelian, then $G$ acts regularly on $V\Gamma$ ,and $G$ is an elementary abelian 2-group.
    

# Section17: Symmetric graphs

## Definitions:

- A graph is t-transitive if its automorphism group is transitive on the set of t-arcs in $G$ ,but not transitive on the set of $(t+1)$\-arcs in $G$.
    

## Propositions:

- If $G$ is a t-transitive graph with girth is $g$ and degree at least 3, then $t\leq\frac{1}{2}(g+2)$.
    
- test for t-transitivity.
    

# Section18: Symmetric graphs of degree three

## Definitions:

## Propositions:

- An automorphism of $G$ which fixes $[\alpha]$, must be the identity.
    
- （Tutte）There is no finite t-transitive cubic graph with $t>5$.
    

# Section19: The covering graph construction

## Definitions:

## Propositions:

- The covering graph $\widetilde{\Gamma}=\widetilde{\Gamma}(K,\theta)$: The vertex-set of $\widetilde{\Gamma}$ is $K\times V\Gamma$ , and two vertices $(\kappa_1,v_1),(\kappa_2,v_2)$ are joined by an edge if and only if $(v_1,v_2)\in S\Gamma$ and  $\kappa_2=\kappa_1\theta(v_1,v_2)$.
    
- There are infinitely many cubic 5-transitive graphs.
    

# Section 20: Distance transitive graph

## Definitions:

- $s_{hi}(u,v)$: The vertices that $d(u,w)=h$ and $d(v,w)=i$.
    
- The intersection numbers: $s_{hji}$.
    
- $k_i$ is the number of vertices in $\Gamma_i(v)$ for any vertex $v$.
    

## Propositions:

- $AA_i=b_{i-1}A_{i-1}+a_i A_i+c_{i+1} A_{i+1}$.
    

  （距离矩阵是邻接矩阵空间的基）

（从基的角度考虑 $s_{hi}(v_r,v_s)$ is depend on the $d(v_r,v_s)$,

# Section21: Feasibility of intersection arrays

## Definitions:

## Propositions:

（左右特征向量的对应关系）

- $m(\lambda_i)=\frac{n}{(u_i,v_i)}$.
    

# Section 23: Minimal regular graphs with given girth

## Definitions:

- The smallest graph with degree $k$ and girth $g$, is a $(k,g)-$ cage.
    

## Propositions:
