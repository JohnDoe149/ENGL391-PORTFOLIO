# ENGL391-PORTFOLIO
My name is John Du, a second-year CS student at UMD (graduation: Spring 2027), and this is my portfolio. This is a brief showcase of 5 of the most important pieces of work I have done so far as well as my general cover letter. I am interested in ML (machine learning) and statistical methods in a variety of domains such as biology but I am now working on ML in robotics. In the future, I want to do research in the field of embodied AI and pursue a PhD.

## Artifact 1: ESM2CPLUSPLUS
A ESM2CPLUSPLUS is a native C++ implementation of Meta labs' protein language model ESM2. ESM2 is a popular BERT (Bidirection Encoding Representations from Transformers) model. I implemented various kinds of transformer architecture and pytorch ML methods such as softmax, multi-head self attention, ROPE (rotary positional embeddings), tokenizer, MLP (multi-layer-perceptron, etc). 

![](/images/esm2.png)
<br> ESM2 architecture showing the pretrained LM (language model) and the protein folding architecture. Paper link: https://www.science.org/doi/10.1126/science.ade2574
![](/images/esm2cpluspluscode.png)
<br> An image of my C++ implementation of multi-head self attention using object-oriented design.
![](/images/transformer.png)
<br> An image of transformer architecture from the original "Attention Is All You Need" paper. Paper link: https://arxiv.org/pdf/1706.03762

## Artifact 2: TIMEINTEGRATEDPHYLOGENETICS
A Bayesian MCMC (Markov Chain Monte Carlo) model using a unique parameterization of "evolutionary time" to try to better handle uncertainty in genomic data. The goal was to handle adversarial datasets better. It does inference on an MSA (multiple sequence alignment) to produce an evolutionary tree. In performance tests, it performed as well as the research standard revBayes in terms of accuracy but had slower convergence and runtime. Model was written in C++. 

![](/images/TIPtrace.png)
<br> An image showing the "fuzzy caterpillar" in the posterior that shows strong exploration of the parameter space for my model.

![](/images/transitionRatePosterior.png)
<br> An image showing the Gaussian-shaped posterior distribution for AC.

<br>Repository link: https://github.com/JohnDoe149/TimeIntegratedPhylogenetics

## Artifact 3: ROBOTWIN-XARM6_UFACTORY_CONFIGURATION
A custom xArm6 configuration for the bimanual robot arm benchmark, RoboTwin. xArm6 is a less commonly used robot arm, so RoboTwin does not have an existing configuration for xArm6 to use to do simulation. Used ROS2 to compile the .urdf and .srdf files and downloaded the meshes. Carefully read the .urdf file and ROS2 documenation to determine important body links. Wrote CuRobo.yml for RoboTwin for simulation purposes.

![](/images/xarm6render.png)
<br> An image showing a 3D render of the xArm6 arm using the .urdf file and associated meshes. Render includes the gripper and the arm body.

## Artifact 4: XARM6_UFACTORY_COLLISION_ANNOTATIONS
Installed and imported the xArm6 mesh and .urdf into Isaac Sim to annotate the collision spheres onto the xArm6 model using Lula. Collision spheres will be used in downstream simulation to avoid self-collision and collision with environment in a computationally efficient manner. 

![](/images/annotatedcollision.png)
<br> An image showing the collision spheres for some of the links of the robot arm.

## Artifact 5: INST123 Database Project
A relational database using PostgresSQL to store important data about popular books across multiple tables. Data includes things like ISBN, Title and Genre. Utilizes relational database features like primary keys and JOINS to do efficient queries. Showed proficency in database administration and query languages like SQL.

![](/images/INST123data.png)
<br> An image showing some of the data in the database from the "Books" table.

## Cover Letter

John Du is a second-year at the UMD (University of Maryland) majoring in computer science (GPA: 3.933) and graduating in the spring of 2027. He is interested in deepRL in robotics, VLAs, software development, and computational modeling.
<br>
As a freshman, he was hired as an undergraduate research assistant for a bioinformatics lab under Prof. Delwiche. He worked on computational modeling, primarily Bayesian inference under Markov Chain Monte Carlo methods. As an independent project, he wrote an evolutionary
history simulation using a novel parameterization. The goal was to see if reparameterizing to try to better handle uncertainty would handle adversarial datasets better. This project was a application of many staples of software development such as unit-testing, compilation,
debugging, and object-oriented design. He performed evaluation with Python scripts and shell
commands to simulate data and compare performance to the standard model, RevBayes.
The reparameterization resulted in the model becoming “stuck” between multiple plausible results, so it ended performing about the same as RevBayes across all datasets. He then worked on an implementation of Meta’s ESM-2 in C++ to gain a deeper understanding
of how BERT and transformer-based models work and to practice software development practices like OOP (Object Oriented Programming) design, version control and Docker. He implemented several key features like multi-head self-attention, rotary embeddings, and tokenization. He also became familiar with concepts like layer normalization and residual connections and developed a strong understanding oftransformer architecture.
<br>
He is now doing research at the CASE lab as a student collaborator, which is headed by Prof.
Ang Li, who is jointly appointed with UMD’s ECE and CS department. Currently, he is
conducting an investigation into twin-arm embodiments and testing different Vision-Language-Action models (VLAs). He is able to apply his past experiences with AI models, Docker and Python to his current research. He is doing simulations on the lab's HPC cluster to evaluate which of the two models (Pi-0.5 and LingbotVLA) can do bimanual tasks better. The model with better performance's pretrained LM (language model) can then be used in another model that would be trained to try and perform more complex bimanual tasks. An example of a complex task would be something like telling the model to make soup; a series of simple instructions (turn on the heat, pour water, etc) that have to be coordinated in advance.