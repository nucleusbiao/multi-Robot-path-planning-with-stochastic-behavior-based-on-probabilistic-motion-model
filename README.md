
# Heterogeneous Multi-Robot Path Planning Based on Probabilistic Motion Model
SBMRPP is based on libMultiRobotPlanning project(https://github.com/whoenig/libMultiRobotPlanning) to slove the multi-Robot path planning with stochastic behavior based on probabilistic motion model.


libMultiRobotPlanning is a library with search algorithms primarily for task and path planning for multi robot/agent systems.
It is written in C++(14), highly templated for good performance, and comes with useful examples.

## Building

Tested on Ubuntu 16.04.

```
mkdir build
cd build
cmake ..
make
```

## Run example instances

### PCBS_ON

````
./PCBS_ON -i ../benchmark/8x8_obst12/map_8by8_obst12_agents7_ex1.yaml -o output.yaml
python3 ../example/visualize.py ../benchmark/8x8_obst12/map_8by8_obst12_agents7_ex1.yaml output.yaml


./PCBS_ON -i ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml -o output.yaml
python3 ../example/visualize.py ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml output.yaml
````

### PCBS_OFF

````
./PCBS_OFF -i ../benchmark/8x8_obst12/map_8by8_obst12_agents7_ex1.yaml -o output.yaml
python3 ../example/visualize.py ../benchmark/8x8_obst12/map_8by8_obst12_agents7_ex1.yaml output.yaml

./PCBS_OFF -i ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml -o output.yaml
python3 ../example/visualize.py ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml output.yaml
````

### PECBS_ON

````
./PECBS_ON -i ../benchmark/8x8_obst12/map_8by8_obst12_agents11_ex1.yaml -o output.yaml -w 1.3
python3 ../example/visualize.py ../benchmark/8x8_obst12/map_8by8_obst12_agents11_ex1.yaml output.yaml

./PECBS_ON -i ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml -o output.yaml -w 1.3
python3 ../example/visualize.py ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml output.yaml
````

### PECBS_OFF

````
./PECBS_OFF -i ../benchmark/8x8_obst12/map_8by8_obst12_agents11_ex1.yaml -o output.yaml -w 1.3
python3 ../example/visualize.py ../benchmark/8x8_obst12/map_8by8_obst12_agents11_ex1.yaml output.yaml

./PECBS_OFF -i ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml -o output.yaml -w 1.3
python3 ../example/visualize.py ../benchmark/32x32_obst204/map_32by32_obst204_agents10_ex1.yaml output.yaml
````

If you use this code, please cite

@article{Hu2020HeterogeneousMP,

  title={Heterogeneous Multi-Robot Path Planning Based on Probabilistic Motion Model},
  
  author={Biao Hu and Haonan Wang and Zhengcai Cao},
  
  journal={2020 IEEE International Conference on Systems, Man, and Cybernetics (SMC)},
  
  year={2020},
  
  pages={1323-1328}
  
}
