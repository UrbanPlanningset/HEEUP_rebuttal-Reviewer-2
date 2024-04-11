# Q2 Supplement  

## Baseline Introduction.

 Existing data-driven energy-efficient urban planning can be divided into four main categories [8,9,10]:

- **Heuristic methods**: This type of method uses algorithms such as genetic algorithm (GA) and particle swarm optimization (PSO) to generate planning solutions that satisfy environmental constraints by simulating natural selection and swarm intelligence.
- **Deep Learning**: Use deep neural networks, such as convolutional neural networks (CNN) or recurrent neural networks (RNN), to process and analyze large-scale urban data to optimize urban layout and energy management.
- **Generative Learning**: Including Generative Adversarial Network (GAN) and Variational Autoencoder (VAE), which generates new urban layout and design plans by learning the distribution of the urban environment.
- **Reinforcement Learning**: Use a reward mechanism to guide the algorithm to make decisions, and continuously optimize the urban planning process to achieve energy conservation.

The specific differences are as follows：

| Category                       | Method              | Decision-making process description                                        | Decision-making perspective       | Characteristics                                             |
|--------------------------------|---------------------|---------------------------------------------------------------------------|-----------------------------------|-------------------------------------------------------------|
| Heuristic                     | Single objective: GA [3] | Simultaneously determine functional areas, building types, and building parameters through iterative optimization | Comprehensive optimization/multi-classification | Finds the optimal solution under environmental constraints, balancing multiple planning goals |
|                                | Multi-objective: MOGA [4], PSO [3,5] | Combines multi-objective optimization strategies to solve the best solution for environmental constraints and planning goals | Comprehensive optimization/multi-objective | Balances environmental constraints and planning goals to find the best balanced solution |
| Deep learning                 | MLP [1,2]                | Utilizes a multi-layer perceptron network to map directly from input features to output planning solutions | Feature mapping/multi-classification | Quickly predicts planning results without a reasoning process |
| Generative learning        | VAE [6], GAN [7]             | Uses adversarial networks to simulate the complexity of urban planning, learning planning solutions through generation and discriminative models | Adversarial generation/sequential generation | Increases the diversity of planning solutions, capturing planning complexity |
| Multi-agent reinforcement learning | COMA              | Uses multi-agent collaborative learning methods to jointly optimize planning decisions based on urban characteristics | Multi-agent collaborative decision-making/collaborative optimization | Collaborative optimization through multi-agent collaboration |
| Hierarchical reinforcement learning | HEEUP            | In line with existing urban planning models, decomposes complex urban planning problems into multi-level sub-problems for processing | Hierarchical collaborative decision-making/hierarchical optimization | Optimization and adjustment between levels to effectively achieve comprehensive energy-saving goals |

**Why compare with COMA?**

In Energy-Efficient Urban Planning, Determine Urban Structure (high-level), Generate Land Use Configuration (mid-level), and Adjust Building Design Parameters (low-level) are three core tasks, which can be intuitively handled by multi-agent RL like COMA, such that each agent takes one task. The reason we choose COMA as a baseline is to validate the necessity and superiority of inherent hierarchical decision-making process  following the top-down schema for Energy-Efficient Urban Planning. 

## Reference
MLP:

- [1] Kusiak, A.; Xu, G.; Zhang, Z. "Minimization of energy consumption in HVAC systems with data-driven models and an interior point method." *Energy Convers. Manag.* 2014, 85, 146–153.

- [2] Ray, M.; Samal, P.; Panigrahi, C.K. "Implementation of a Hybrid Technique for the Predictive Control of the Residential Heating Ventilation and Air Conditioning Systems." *Eng. Technol. Appl. Sci. Res.* 2022, 12, 8772–8776.

GA, PSO, MOGA:

- [3] Bouktif, S.; Fiaz, A.; Ouni, A.; Serhani, M.A. "Multi-sequence LSTM-RNN deep learning and metaheuristics for electric load forecasting." *Energies* 2020, 13, 391.

- [4] Ding, Y.; Zhang, Q.; Yuan, T. "Research on short-term and ultra-short-term cooling load prediction models for office buildings." *Energy Build.* 2017, 154, 254–267.

- [5] Chen, S.; Zhou, X.; Zhou, G.; Fan, C.; Ding, P.; Chen, Q. "An online physical-based multiple linear regression model for building’s hourly cooling load prediction." *Energy Build.* 2022, 254, 111574.


VAE, GAN:
- [6]  Wang, Dongjie et al. "Reimagining city configuration: Automated urban planning via adversarial learning." In *Proceedings of the 28th International Conference on Advances in Geographic Information Systems*, 497–506, 2020.
- [7]  Wang, Dongjie et al. "Automated urban planning for reimagining city configuration via adversarial learning: quantification, generation, and evaluation." *ACM Transactions on Spatial Algorithms and Systems* 9.1 (2023): 1–24.

## References on algorithm classification:
- [8]  Olu-Ajayi, Razak et al. "Data-driven tools for building energy consumption prediction: A review." *Energies* 16.6 (2023): 2574. MDPI.
- [9]  Amasyali, Kadir and El-Gohary, Nora M. "A review of data-driven building energy consumption prediction studies." *Renewable and Sustainable Energy Reviews* 81 (2018): 1192–1205. Elsevier.
- [10] Liu, Huiheng, Liang, Jinrui, Liu, Yanchen, and Wu, Huijun. "A review of data-driven building energy prediction." *Buildings* 13.2 (2023): 532. MDPI.
## References on energy efficiency:
-  [11] Klemm, Christian and Wiese, Frauke. "Indicators for the optimization of sustainable urban energy systems based on energy system modeling." *Energy, Sustainability and Society* 12.1 (2022): 3. Springer. 
