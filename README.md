# Privacy-Preserved-Aggregate-Thermal-Dynamic-Model-for-Building-Cluster
# This program is implemented in the following environment:
1. Matlab 2022b
2. Gurobi Optimizer version 10.0.2
3. Yalmip version 20220622
# Fire description
1. <non_privacy_preserved_algorithm.m> is the benchmark algorithm, solving the parameter estimation problem of the aggregate thermal dynamic model (ATDM) through the block coordinate descent method  (BCDM).
2. <privacy_preserved_algorithm.m> solves the parameter estimation problem of the ATDM, while protecting the sensitive data of agents, including the indoor temperature and heating/cooling power.
3. <myFun_GetValue.m> is a tool function that can transform the 'sdpvar' to 'value'.
4. <welldata.mat> is the raw data, containing the information of buildings and their surrounding environment.
5. <npp_data.mat> records the results of running <non_privacy_preserved_algorithm.m>.
6. <pp_data.mat> records the results of running <privacy_preserved_algorithm.m>.
7. <result.m> outputs the final results.
# How to run 
1. The readers can simply run <result.m> to obtain the final results.
2. The readers can run <privacy_preserved_algorithm.m> and <non_privacy_preserved_algorithm.m> to obtain optimization calculation results and perform drawing according to your their needs.
