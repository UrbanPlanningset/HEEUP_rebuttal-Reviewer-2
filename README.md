# Q2 Supplement  

## Baseline Introduction.

 Existing data-driven energy-efficient urban planning can be divided into four main categories [11,12,13]:

- **Heuristic methods**: This type of method uses algorithms such as genetic algorithm (GA) and particle swarm optimization (PSO) to generate planning solutions that satisfy environmental constraints by simulating natural selection and swarm intelligence.
- **Deep Learning**: Use deep neural networks to process and analyze large-scale urban data to optimize urban layout and energy management.
- **Generative Learning**: Including Generative Adversarial Network (GAN) and Variational Autoencoder (VAE), which generates new urban layout and design plans by learning the distribution of the urban environment.
- **Reinforcement Learning**: Use a reward mechanism to guide the algorithm to make decisions, and continuously optimize the urban planning process to achieve energy conservation.

The specific differences are as follows：

| Category                       | Method              | Decision-making process description                                        | Decision-making perspective       | Characteristics                                             |
|--------------------------------|---------------------|---------------------------------------------------------------------------|-----------------------------------|-------------------------------------------------------------|
| Heuristic                     | Single objective: GA [4] | Simultaneously determine functional areas, building types, and building parameters through iterative optimization | Comprehensive optimization/multi-classification | Finds the optimal solution under environmental constraints, balancing multiple planning goals |
|                                | Multi-objective: MOGA [6], PSO [5] | Combines multi-objective optimization strategies to solve the best solution for environmental constraints and planning goals | Comprehensive optimization/multi-objective | Balances environmental constraints and planning goals to find the best balanced solution |
| Deep learning                 | MLP [1,2,3]                | Utilizes a multi-layer perceptron network to map directly from input features to output planning solutions | Feature mapping/multi-classification | Quickly predicts planning results without a reasoning process |
| Generative learning        | VAE [7], GAN [8]             | Uses adversarial networks to simulate the complexity of urban planning, learning planning solutions through generation and discriminative models | Adversarial generation/sequential generation | Increases the diversity of planning solutions, capturing planning complexity |
| Multi-agent reinforcement learning | COMA              | Uses multi-agent collaborative learning methods to jointly optimize planning decisions based on urban characteristics | Multi-agent collaborative decision-making/collaborative optimization | Collaborative optimization through multi-agent collaboration |
| Hierarchical reinforcement learning | HEEUP            | In line with existing urban planning models, decomposes complex urban planning problems into multi-level sub-problems for processing | Hierarchical collaborative decision-making/hierarchical optimization | Optimization and adjustment between levels to effectively achieve comprehensive energy-saving goals |

**Why compare with COMA?**

In Energy-Efficient Urban Planning, Determine Urban Structure (high-level), Generate Land Use Configuration (mid-level), and Adjust Building Design Parameters (low-level) are three core tasks, which can be intuitively handled by multi-agent RL like COMA, such that each agent takes one task. The reason we choose COMA as a baseline is to validate the necessity and superiority of inherent hierarchical decision-making process  following the top-down schema for Energy-Efficient Urban Planning. 

## Reference
MLP:

- [1] Kusiak, A.; Xu, G.; Zhang, Z. "Minimization of energy consumption in HVAC systems with data-driven models and an interior point method." *Energy Convers. Manag.* 2014, 85, 146–153.

- [2] Ray, M.; Samal, P.; Panigrahi, C.K. "Implementation of a Hybrid Technique for the Predictive Control of the Residential Heating Ventilation and Air Conditioning Systems." *Eng. Technol. Appl. Sci. Res.* 2022, 12, 8772–8776.

- [3] Chen, S.; Zhou, X.; Zhou, G.; Fan, C.; Ding, P.; Chen, Q. "An online physical-based multiple linear regression model for building’s hourly cooling load prediction." *Energy Build.* 2022, 254, 111574.

GA, PSO, MOGA:

- [4] Ooka, R., & Komamura, K. (2009). Optimal design method for building energy systems using genetic algorithms. *Building and Environment, 44*(7), 1538-1544. Elsevier.

- [5] Elsheikh, A. H., & Abd Elaziz, M. (2019). Review on applications of particle swarm optimization in solar energy systems. *International Journal of Environmental Science and Technology, 16*, 1159-1170. Springer.

- [6] Costa-Carrapiço, I., Raslan, R., & González, J. N. (2020). A systematic review of genetic algorithm-based multi-objective optimisation for building retrofitting strategies towards energy efficiency. *Energy and Buildings, 210*, 109690. Elsevier.


VAE, GAN:
- [7]  Wang, Dongjie et al. "Reimagining city configuration: Automated urban planning via adversarial learning." In *Proceedings of the 28th International Conference on Advances in Geographic Information Systems*, 497–506, 2020.
- [8]  Wang, Dongjie et al. "Automated urban planning for reimagining city configuration via adversarial learning: quantification, generation, and evaluation." *ACM Transactions on Spatial Algorithms and Systems* 9.1 (2023): 1–24.

## References on algorithm classification:
- [9]  Olu-Ajayi, Razak et al. "Data-driven tools for building energy consumption prediction: A review." *Energies* 16.6 (2023): 2574. MDPI.
- [10]  Amasyali, Kadir and El-Gohary, Nora M. "A review of data-driven building energy consumption prediction studies." *Renewable and Sustainable Energy Reviews* 81 (2018): 1192–1205. Elsevier.
- [11] Liu, Huiheng, Liang, Jinrui, Liu, Yanchen, and Wu, Huijun. "A review of data-driven building energy prediction." *Buildings* 13.2 (2023): 532. MDPI.
## References on energy efficiency:
-  [12] Klemm, Christian and Wiese, Frauke. "Indicators for the optimization of sustainable urban energy systems based on energy system modeling." *Energy, Sustainability and Society* 12.1 (2022): 3. Springer. 
