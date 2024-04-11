# Q2 Supplement  HEEUP vs Baseline.
 
| Category                       | Method              | Decision-making process description                                        | Decision-making perspective       | Characteristics                                             |
|--------------------------------|---------------------|---------------------------------------------------------------------------|-----------------------------------|-------------------------------------------------------------|
| Heuristic                     | Single objective: GA | Simultaneously determine functional areas, building types, and building parameters through iterative optimization | Comprehensive optimization/multi-classification | Finds the optimal solution under environmental constraints, balancing multiple planning goals |
|                                | Multi-objective: MOGA, PSO | Combines multi-objective optimization strategies to solve the best solution for environmental constraints and planning goals | Comprehensive optimization/multi-objective | Balances environmental constraints and planning goals to find the best balanced solution |
| Deep learning                 | MLP                 | Utilizes a multi-layer perceptron network to map directly from input features to output planning solutions | Feature mapping/multi-classification | Quickly predicts planning results without a reasoning process |
| Adversarial generation        | VAE/GAN             | Uses adversarial networks to simulate the complexity of urban planning, learning planning solutions through generation and discriminative models | Adversarial generation/sequential generation | Increases the diversity of planning solutions, capturing planning complexity |
| Multi-agent reinforcement learning | COMA              | Uses multi-agent collaborative learning methods to jointly optimize planning decisions based on urban characteristics | Multi-agent collaborative decision-making/collaborative optimization | Collaborative optimization through multi-agent collaboration |
| Hierarchical reinforcement learning | HEEUP            | In line with existing urban planning models, decomposes complex urban planning problems into multi-level sub-problems for processing | Hierarchical collaborative decision-making/hierarchical optimization | Optimization and adjustment between levels to effectively achieve comprehensive energy-saving goals |

MLP:
- Kusiak, A.; Xu, G.; Zhang, Z. "Minimization of energy consumption in HVAC systems with data-driven models and an interior point method." *Energy Convers. Manag.* 2014, 85, 146–153.
- Ray, M.; Samal, P.; Panigrahi, C.K. "Implementation of a Hybrid Technique for the Predictive Control of the Residential Heating Ventilation and Air Conditioning Systems." *Eng. Technol. Appl. Sci. Res.* 2022, 12, 8772–8776.

GA, PSO, MOGA:
- Bouktif, S.; Fiaz, A.; Ouni, A.; Serhani, M.A. "Multi-sequence LSTM-RNN deep learning and metaheuristics for electric load forecasting." *Energies* 2020, 13, 391.
- Ding, Y.; Zhang, Q.; Yuan, T. "Research on short-term and ultra-short-term cooling load prediction models for office buildings." *Energy Build.* 2017, 154, 254–267.
- Chen, S.; Zhou, X.; Zhou, G.; Fan, C.; Ding, P.; Chen, Q. "An online physical-based multiple linear regression model for building’s hourly cooling load prediction." *Energy Build.* 2022, 254, 111574.

VAE, GAN:
- Wang, Dongjie et al. "Reimagining city configuration: Automated urban planning via adversarial learning." In *Proceedings of the 28th International Conference on Advances in Geographic Information Systems*, 497–506, 2020.
- Wang, Dongjie et al. "Automated urban planning for reimagining city configuration via adversarial learning: quantification, generation, and evaluation." *ACM Transactions on Spatial Algorithms and Systems* 9.1 (2023): 1–24.

References on algorithm classification:
- Olu-Ajayi, Razak et al. "Data-driven tools for building energy consumption prediction: A review." *Energies* 16.6 (2023): 2574. MDPI.
- Amasyali, Kadir and El-Gohary, Nora M. "A review of data-driven building energy consumption prediction studies." *Renewable and Sustainable Energy Reviews* 81 (2018): 1192–1205. Elsevier.

References on energy efficiency:
- Klemm, Christian and Wiese, Frauke. "Indicators for the optimization of sustainable urban energy systems based on energy system modeling." *Energy, Sustainability and Society* 12.1 (2022): 3. Springer. 
