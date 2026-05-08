# ENGL391-PORTFOLIO
My Name is John Du, a second-year CS student at UMD (graduation: Spring 2027), and this is my portfolio. This is a brief showcase of 5 of the most important work I have done so far during University. I am interested in Machine Learning and Applied Statistics methods in a variety of domains such as biology but I am now working on Machine Learning in applied robotics. 
## Artifact 1: ESM2CPLUSPLUS
A ESM2CPLUSPLUS is a native C++ implementation of Meta labs' protein language model ESM2. ESM2 is a popular BERT (Bidirection Encoding Representations from Transformers) model. I implemented many of the pytorch ML methods such as softmax, GELU, multi-head self attention, ROPE (rotary positional embeddings), tokenizer, MLP (multi-layer-percepatron, etc). 

![](/images/esm2.png)
<br> ESM2 architecture showing the pretrained LM (language model) and the protein folding architecture. Paper link: https://www.science.org/doi/10.1126/science.ade2574
![](/images/esm2cpluspluscode.png)
<br> An image of my C++ implementation of multi-head self attention using object-oriented design
![](/images/transformer.png)
<br> An image of transformer architecture from the original "Attention Is All You Need" paper. Paper link: https://arxiv.org/pdf/1706.03762

## Artifact 2: TIMEINTEGRATEDPHYLOGENETICS
A Bayesian MCMC (Markov Chain Monte Carlo) model using a unique parameterization of "evolutionary time" to try to better handle uncertainty in genomic data to handle adversarial datasets better. It does inference from an MSA (multiple sequence alignment) to produce an evolutionary tree. In performance tests, it performed as well research standard revBayes in terms of accuracy but had slower convergence and runtime. Model was written in C++. 

![](/images/TIPtrace.png)
<br> An image showing the "fuzzy caterpillar" in the posterior trace file that shows strong exploration of the parameter space for my model.

![](/images/transitionRatePosterior.png)
<br> An image showing the Gaussian-shaped posterior distribution for AC.

<br>Repository link: https://github.com/JohnDoe149/TimeIntegratedPhylogenetics

## Artifact 3: ROBOTWIN-XARM6_UFACTORY_CONFIGURATION
A custom xArm6 configuration for the bimanual robot arm benchmark, RoboTwin. xArm6 is a less commonly used arm and so RoboTwin does not have a configuration for xArm6 to use to do simulation. Used ROS2 to compile the .urdf and .srdf files and downloaded the meshes. Carefully read the .urdf file and ROS2 documenation to determine important body links. Wrote CuRobo.yml for RoboTwin to simulate the xArm6.

## Artifact 4: XARM6_UFACTORY_COLLISION_ANNOTATIONS
Installed and imported the xArm6 mesh and .urdf into Isaac Sim to annotate the collision spheres onto the xArm6 model using Lula. Manually edited each link's collision spheres to improve downstream simulation.

## Artifact 5: INST123 Database Project
A relational database using PostgresSQL to store important data about popular books across multiple tables. Data includes things like ISBN, Title and Genre. Utilizes relational database features like primary keys and JOINS to do efficient queries. Showed proficency in database administration and query languages like SQL.

![](/images/INST123data.png)
<br> An image showing some of the data in the database from the "Books" Table.
## Cover Letter
