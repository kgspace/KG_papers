# Mathematics Spaces for Machine Learning
We aim to summary the Machine Learning Models from the perspective of Math Spaces, like Euclidean Space, Banach Space, Manifold...
Also, we try to explain the advantages and disadvantages in different Maths Spaces.

## Definition of Spaces and the relationship between them
<img src="https://github.com/kgspace/KG_papers/blob/main/images/spaces%20relation.png" width="600" height="300" align="center" >

## Learning in Different Mathematical Spaces
### Learning in Banach spaces 
- Firstly, there is essentially only one Hilbert space once the dimension of the space is fixed. This follows from the well-known fact that any two Hilbert
spaces over C of the same dimension are isometrically isomorphic. Thus, compared to Hilbert spaces, Banach spaces possess much richer geometric structures, which are potentially useful for developing learning algorithms.
- Secondly, in some applications, a norm from a Banach space is invoked without being induced from an inner product.
- Thirdly, since many training data come with intrinsic structures that make them impossible to be embedded into a Hilbert space, learning algorithms based on RKHS may not work well for them.                
-----------------------------------cited from **Reproducing Kernel Banach Spaces for Machine Learning 2009**

### Learning in Hyperbolic Space
- One of the defining characteristics of hyperbolic space is that it is in some sense larger than the more familiar Euclidean space; the area of a circle or volume of a sphere grows exponentially with its radius, rather than polynomially. This suggests that low-dimensional hyperbolic spaces may provide effective representations of data in ways that low-dimensional Euclidean spaces cannot. ------cited from **Neural Embeddings of Graphs in Hyperbolic Space 2017**
- Hyperbolic space can be thought of as a continuous version of trees and as such it is naturally equipped to model **hierarchical structures.** For instance, it has been shown that any finite tree can be embedded into a finite hyperbolic space such that distances are preserved approximately. ----cited from **Poincaré Embeddings for Learning Hierarchical Representations 2017**


## Survey Paper
1. **A Survey of Topological Machine Learning Methods.**
*Felix Hensel, Michael Moor and Bastian Rieck* *  Frontiers in Artificial Intelligence 2021 [[paper]](https://www.frontiersin.org/articles/10.3389/frai.2021.681108/full)


## Journal and Conference Paper

### Metric Space 

### Normed Space 
- ### Banach Space
1. **Separating theorem of samples in Banach space for support vector machine learning.** *Qiang He and Congxin Wu.* International Journal of Machine Learning and Cybernetics [[paper]](https://link.springer.com/article/10.1007/s13042-011-0013-4)

1. **Reproducing Kernel Banach Spaces for Machine Learning.** *Haizhang Zhang, Yuesheng Xu, Jun Zhang.* Journal of Machine Learning Research 2009 
[[paper]](https://www.jmlr.org/papers/volume10/zhang09b/zhang09b.pdf)






### Vector Space 
- ### Euclidean Space
- ### Hilbert Space
1. **Quantum machine learning in feature Hilbert spaces.** *Maria Schuld, Nathan Killoran.* Physical review letters 2019 
[[paper]](https://arxiv.org/abs/1803.07128)

1. **Hilbert Space Embeddings of Conditional Distributions with Applications to Dynamical Systems.** *Le Song, Jonathan Huang, Alex Smola, Kenji Fukumizu.*
ICML 2009 [[paper]](https://dl.acm.org/doi/abs/10.1145/1553374.1553497)




### Topological Space
1. **A Stable Multi-Scale Kernel for Topological Machine Learning.** *Jan Reininghaus, Stefan Huber, Ulrich Bauer, Roland Kwitt.*  
CVPR 2015 [[paper]](https://openaccess.thecvf.com/content_cvpr_2015/papers/Reininghaus_A_Stable_Multi-Scale_2015_CVPR_paper.pdf)

1. **Machine learning topological states.** *Dong-Ling Deng, Xiaopeng Li, and S. Das Sarma.* Physical Review B 2017 
[[paper]](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.96.195145)

1. **Machine-Learning-Based Hotspot Detection Using Topological Classification and Critical Feature Extraction.** *Yen-Ting Yu, Geng-He Lin, Iris Hui-Ru Jiang, Charles Chiang.* IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems 2015 
[[paper]](https://ieeexplore.ieee.org/abstract/document/7001593)
- ### Manifold 
1. **Manifold for Machine Learning Assurance.** 
*Taejoon Byun, Sanjai Rayadurgam.* ICSE-NIER 2020 [[paper]](https://ieeexplore.ieee.org/abstract/document/9397537)

1. **Poincaré Embeddings for Learning Hierarchical Representations.** *Maximilian Nickel, Douwe Kiela* NeurlPS 2017 [[paper]](https://arxiv.org/abs/1705.08039)

1. **POINCAR´E GLOVE: HYPERBOLICWORD EMBEDDINGS.** *Alexandru Tifrea, Gary B´ecigneul, Octavian-Eugen Ganea* ICLR 2019 [[paper]](https://arxiv.org/abs/1810.06546)

1. **Neural Embeddings of Graphs in Hyperbolic Space.** *Benjamin Paul Chamberlain, James Clough, Marc Peter Deisenroth* KDD 2017 [[paper]](https://arxiv.org/abs/1705.10359)

### Other Special Spaces




