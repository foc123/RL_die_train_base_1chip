# RL_die_train_base_1chip

RL_train.tar用于训练，RL_infer.tar用于推测。  
decap_ppo_demo.py是单次训练的code，ray_demo.py是进行大规模训练的文件  
decap_ppo_demo.py中，multi代表样本训练的个数，范围为1-10。  
这个代码针对是chip中其中一个core的vdi优化，在覆盖core的pdn网络中选择10个节点放置decap，infer.tar中result_fig有case6的参考结果。  
其中包括优化的decap选择（每个cap容值为数值*0.1nF），reward值。  
