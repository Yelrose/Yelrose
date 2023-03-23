### Hi, I'm Yelrose! 👋
I am a master major in computer science and graduated from Sun Yat-sen University, and currently working at Baidu with a focus on graph neural networks and natural language processing.

### My Work
I have worked on many cool projects at Baidu, and have had the opportunity to use my expertise in graph neural networks to develop cutting-edge solutions. Here are a few highlights:

- Created PGL, a graph neural network framework based on PaddlePaddle. With PGL, you can easily build and train graph neural networks. Check out the sample code below:

```python
import pgl

g = pgl.Graph(num_nodes=num_nodes, edges=edges, node_feat={"h": feature})
g.tensor()

def send_func(src_feat, dst_feat, edge_feat):
    return src_feat

def recv_func(msg):
    return msg.reduce_sum(msg["h"]) 

msg = g.send(send_func, src_feat=g.node_feat)
ret = g.recv(recv_func, msg)
```
- With PGL, we developed [TransformerConv](https://arxiv.org/abs/2009.03509), a novel graph neural network architecture that has achieved top performance on multiple OGB benchmarks, as well as winning first place at [KDD Cup 2021](https://ogb.stanford.edu/paper/kddcup2021/mag240m_BD-PGL.pdf) and [NeurIPS 2022 OGB-LSC](https://ogb.stanford.edu/paper/neurips2022/mag240m_ComeAgain.pdf). 

- Our teams created two powerful tools, [Graph4Rec](https://arxiv.org/abs/2112.01035) and PGLBox ([Github links](https://github.com/PaddlePaddle/PGL/tree/main/apps/PGLBox)), for running recommender systems with graph neural networks. 

- We applied graph neural networks to a variety of applications, including [geographic location search](https://dl.acm.org/doi/10.1145/3447548.3467059), [ETA prediction](https://arxiv.org/abs/2208.06979), and [cross-modal document understanding](https://arxiv.org/abs/2209.08569).


If you are interested in collaborating with me or interning at Baidu, feel free to send me an email at huangzhengjie@baidu.com.


![Language](https://github-readme-stats.vercel.app/api/top-langs/?username=Yelrose&layout=compact)

![Yelrose's GitHub stats](https://github-readme-stats.vercel.app/api?username=Yelrose&show_icons=true&theme=radical)

