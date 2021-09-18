# Mathematics Spaces for Machine Learning
We aim to summary the Machine Learning Models from the perspective of Math Spaces, like Euclidean Space, Banach Space, Manifold...
Also, we try to explain the advantages and disadvantages in different Maths Spaces.

## Definition of Spaces and the relationship between them
- ### Metric Space

<img src="https://github.com/kgspace/KG_papers/blob/main/images/metric%20space.png" width="600" align="center" >

- ### Normed Space
- <img src="https://github.com/kgspace/KG_papers/blob/main/images/normed%20space.png" width="600" align="center" >

- ### Inner Product Space
<img src="https://github.com/kgspace/KG_papers/blob/main/images/Inner%20Product%20Space.png" width="600" align="center" >

- ### Topological Space
<img src="https://github.com/kgspace/KG_papers/blob/main/images/Topological%20Space.png" width="600" align="center" >

- ### Relationship

<img src="https://github.com/kgspace/KG_papers/blob/main/images/spaces%20relation.png" width="600" height="300" align="center" >
<img src="https://github.com/kgspace/KG_papers/blob/main/images/spaces%20relation2.png" width="400" align="center" >
<img src="https://github.com/kgspace/KG_papers/blob/main/images/spaces%20relation4.png" width="400" align="center" >
<img src="https://github.com/kgspace/KG_papers/blob/main/images/spaces%20relation3.png" width="600" align="center" >

- ### Properties

## Advantages and Disadvantages of Different Maths Spaces

### Euclidean Space
**Disadvantages**
- **Ill-posed algebraic system**  As is the case that triples are much more than the sum of entities and relations, the number of variables are much less than the number of equations, which is typically an illposed algebraic system. Mathematically, an ill-posed algebraic system would commonly make the solutions imprecise and unstable.
- **Over-strict geometric form** When many tail entities compete for only one point, there would be a major loss of objective function. -----from **Manifold**


### Hilbert Space 
**Advantages**
- **Infinite** A Hilbert space might be infinite dimensional, but just like in R^n, we can talk about independent sets, orthogonality and bases. We can also project, decompose, linearly transform and everything else we can do in Euclidean space. Most practical computations in Hilbert spaces boil down to ordinary linear algebra.
- **Bilinear Inner Product** The geometry of Hilbert spaces is well understood, and the bilinearity of the inner-product makes a thorough-going analysis possible.
- **Self-dual** Hilbert spaces are self-dual. The dual space is also complete so it is a Hilbert space in its own right.
- **Kernal Method** 
- **Angel can be defined by inner product**
- **Basic of Quantum Mechanics** The concept of Hilbert space is the mathematical underpinning of quantum mechanics, and the whole concept of quantum mechanics is discussed in this Hilbert space.The state vector that represents the state of a particle in quantum mechanics is an element in Hilbert space.

**Disadvantages**
- **The definition of distance is unnatural** Most data do not come with any natural notion distance that can be induced from an inner-product. 距离由内积产生，很不自然
- **Only one Hilbert Space** All Euclidean spaces of the same basis cardinality are isometrically isomorphic, there is, in a sense, only one inner-product space. 本质上只有一个希尔伯特空间



### Banach Space
**Advantages**
- **Rich Geometric Structures** Banach spaces possess much richer geometric structures, which are potentially useful for developing learning algorithms.
- **Uniformly smooth and Uniformly convex** A norm from a Banach space is invoked without being induced from an inner product. Banach spaces: the uniformly smooth and uniformly convex spaces.

### Topological Space
**Advantages**
- **Multi-scale, global, and intrinsic properties** As a complement to localised and generally more rigid geometric features, topological features are suitable to capture multi-scale, global, and intrinsic properties of data sets.  Instead of restricting the analysis to statistical descriptors, topological data analysis (TDA) aims to analyse data from a fundamentally different perspective by investigating this underlying manifold structure in an algebraic fashion.   ----from **A Survey of Topological Machine Learning Methods**

- **Well-posed algebraic system** 
- **CLear geometric form** ManifoldE alleviates this issue by expanding the position of golden triples from one point to a manifold such as a high-dimensional sphere. By this mean, ManifoldE avoids much noise to distinguish the true facts from the most possible false ones.       ----from **ManifoldE**

### Group
**Advantages**
- **Never diverge unlimitedly** By choosing a compact Lie group as an embedding space, embeddings never diverge unlimitedly and regularization is no longer required.
- **More scalable** TorusE is more scalable to large-size knowledge graphs because its complexity is the lowest compared with other methods, and we show that it is faster than TransE empirically because of the reduced calculation times without regularization.   ------ from **TorusE**

- **Capture relation compositions.**
- **Capture all desired properties**    -----from DihEdral


## Learning in Different Mathematical Spaces

### Learning in Hilbert Space
Hilbert space embeddings of conditional distributions are potentially useful in applications where conditional distributions are the key quantities of interest, such as regressing structured response variables. -------cited from **Hilbert Space Embeddings of Conditional Distributions
with Applications to Dynamical Systems.**

### Learning in Banach space
- Firstly, there is essentially only one Hilbert space once the dimension of the space is fixed. This follows from the well-known fact that any two Hilbert
spaces over C of the same dimension are isometrically isomorphic. Thus, compared to Hilbert spaces, Banach spaces possess much richer geometric structures, which are potentially useful for developing learning algorithms.
- Secondly, in some applications, a norm from a Banach space is invoked without being induced from an inner product.
- Thirdly, since many training data come with intrinsic structures that make them impossible to be embedded into a Hilbert space, learning algorithms based on RKHS may not work well for them.                
-----------------------------------cited from **Reproducing Kernel Banach Spaces for Machine Learning 2009**

### Learning in Topological(Hyperbolic) Space
- One of the defining characteristics of hyperbolic space is that it is in some sense larger than the more familiar Euclidean space; the area of a circle or volume of a sphere grows exponentially with its radius, rather than polynomially. This suggests that low-dimensional hyperbolic spaces may provide effective representations of data in ways that low-dimensional Euclidean spaces cannot. ------cited from **Neural Embeddings of Graphs in Hyperbolic Space 2017**
- Hyperbolic space can be thought of as a continuous version of trees and as such it is naturally equipped to model **hierarchical structures.** For instance, it has been shown that any finite tree can be embedded into a finite hyperbolic space such that distances are preserved approximately. ----cited from **Poincaré Embeddings for Learning Hierarchical Representations 2017**

### Learning in Probability Space
- In this article, we want to show how both linear and nonlinear dependence in collected data can be exploited in a different latent space, in detail, the uniform probability space (UPS).This enables a deeper understanding of the underlying true distribution. Linear transformation schemes, copulas, and noncomplex neural network architectures are good candidates for such a purpose.  ----------cited from **Segmented Generative Networks: Data Generation in the Uniform Probability Space**
- Formalizing and solving optimization problems over such —infinite dimensional, non-euclidean— probability spaces is conceptually challenging. In this work, we do so by means of gradient flows, a linchpin of applied mathematics for modeling dynamics in very general infinitedimensional spaces. -----cited from **Dataset Dynamics via Gradient Flows in Probability Space**


## Related Work



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






### Inner Product Space 
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

- ### Hyperspherical Space(n-sphere)
1. **Machine Learning Analysis of Complex Networks in Hyperspherical Space.** *María Pereda, Ernesto Estrada.* Physics and Society 2018 
[[paper]](https://arxiv.org/abs/1804.05960)

- ### Manifold 

1. **Machine learning meets complex networks via coalescent embedding in the hyperbolic space.** *Alessandro Muscoloni, Josephine Maria Thomas, Sara Ciucci, Ginestra Bianconi & Carlo Vittorio Cannistraci.* Nature Communications 2017 [[paper]](https://www.nature.com/articles/s41467-017-01825-5)

1. **Manifold for Machine Learning Assurance.** 
*Taejoon Byun, Sanjai Rayadurgam.* ICSE-NIER 2020 [[paper]](https://ieeexplore.ieee.org/abstract/document/9397537)

1. **Poincaré Embeddings for Learning Hierarchical Representations.** *Maximilian Nickel, Douwe Kiela* NeurlPS 2017 [[paper]](https://arxiv.org/abs/1705.08039)

1. **POINCAR´E GLOVE: HYPERBOLICWORD EMBEDDINGS.** *Alexandru Tifrea, Gary B´ecigneul, Octavian-Eugen Ganea* ICLR 2019 [[paper]](https://arxiv.org/abs/1810.06546)

1. **Neural Embeddings of Graphs in Hyperbolic Space.** *Benjamin Paul Chamberlain, James Clough, Marc Peter Deisenroth* KDD 2017 [[paper]](https://arxiv.org/abs/1705.10359)

### Probability Space
1. **Segmented Generative Networks: Data Generation in the Uniform Probability Space.** *Nunzio A.Letizia, Andrea M.Tonello.* IEEE Transactions on Neural Networks and Learning Systems 2020 [[paper]](https://ieeexplore.ieee.org/abstract/document/9298471)

1. **Dataset Dynamics via Gradient Flows in Probability Space.** *David Alvarez-Melis, Nicolò Fusi.*  PMLR 2021 
[[paper]](https://proceedings.mlr.press/v139/alvarez-melis21a.html)

### Other Special Spaces

- ### Complex Vector Space
1. **RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space.** *Zhiqing Sun, Zhi-Hong Deng, Jian-Yun Nie, Jian Tang.* ICLR 2019
[[paper]](https://arxiv.org/abs/1902.10197)

1. **Quaternion Neural Networks for Spoken Language Understanding** 


- ### Polar Coordinates Space

### Other Machine Learning Methods
- ### Geometric Machine Learning
1. **Geometric Deep Learning: Grids, Groups, Graphs, Geodesics, and Gauges.** *Michael M. Bronstein, Joan Bruna, Taco Cohen, Petar Veličković.*
arXiv 2021 [[paper]](https://arxiv.org/abs/2104.13478)

- ### Quantum Machine Learning
1. **Advances in quantum machine learning.** *Jeremy Adcock, Euan Allen, Matthew Day, Stefan Frick, Janna Hinchliff, Mack Johnson, Sam Morley-Short, Sam Pallister, Alasdair Price, Stasja Stanisic.* Quantum Physics 2015 [[paper]](https://arxiv.org/abs/1512.02900)

1. **Quantum machine learning.** *Jacob Biamonte, Peter Wittek, Nicola Pancotti, Patrick Rebentrost, Nathan Wiebe & Seth Lloyd.* Nature 2017
[[paper]](https://www.nature.com/articles/nature23474)


