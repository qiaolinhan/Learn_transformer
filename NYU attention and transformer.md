# [Practicum: Attention and Transformer](https://www.youtube.com/watch?v=f01J0Dri-6k)
> NYU spring 2020  
Attention (self/ cross; hard/ soft) -- dealing with sets (transformers are maps of sets to sets)
__They do not really deal with Seq2Seq, they can be write as order set, but do not nessessarily need to have order sequences__  
## Self Attention I
$$\lbrace x_i \rbrace ^t_{i=1} = \lbrace x_1, x_2, x_3, \cdots, x_t \rbrace\ \ \ \ x_i \in \textrm{R}^n$$
The hidden representation os going to be a linear combination of these vectors (through matrix multiplication)  
$$h = \alpha_1 x_1 + \alpha_2 x_2 + \cdots + \alpha_t x_t = Xa \in \textrm{R}$$
Hard attention: impose that the zero norm of these $a$ vector equals to 1, which means the $a$ is a one hot vector  
$$\Vert a \Vert_0 = 1$$
Soft attention: The constraint is that the summation of these elements all by $\alpha$s, they have to sum to one. ($h$ is the combination of the columns of the matrix $X$)   
$$\Vert a \vert_1 = 1$$  

## Self Attention II
$$a = [soft] (arg)max_{\beta} (X^{\top}x) \in \textrm{R}^t$$
where $\beta$ is the parameterfor the soft arg max
$$\lbrace x_i \rbrace^t_{i=1} \mapsto \lbrace a_i \rbrace^t_{i=1} \mapsto A \in \textrm{R}^{t \times t}$$  

## K-value Store  
About the data structure
* Paradigm for 
  * storing (saving) 
  * retriving (querying)
  * managing
