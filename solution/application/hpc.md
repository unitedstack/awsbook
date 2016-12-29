> ### **High Performance Computing**

几种类型的高性能计算 High Performance Computing：

1. Loosely Coupled Grid Computing

 * 计算节点之间的互相依赖和交互不多，节点更多的是独立完成一部分任务，因此能够容忍节点的失效或动态增加。例如金融风险分析中的 Monte Carlo 仿真
 
 * 适合采用 Amazon EC2 Spot Instance，以及 Auto Scaling
 
 * 对于可以充分利用 GPU 加速的应用，还可以选择 Amazon EC2 G2 instances 配合 NVIDIA’s CUDA 并行计算或 OpenCL 使用

2. Tightly Coupled HPC

 * 计算节点的任务之间有很强的关联性，这列应用通常是基于 messaging passing interface (MPI) 编写的，节点之间有大量的通信，因此对节点间通信的延迟很敏感，也不能容忍节点的失效。例如气象模型仿真、计算流体力学
 
 * 适合采用 Amazon EC2 placement groups 和  enhanced networking，以减少节点间的网络延迟
 
 * 也可采用 GPU instance

3. Data-Intensive Computing

 * 计算过程中需要处理大量数据的，但与大数据应用有区别，处理的是 well-structured data models，例如对一个物理形状的 3D 网格数据处理，或者对一个动漫的独立帧处理
 
 * 可以采用 Amason S3、Amazon EBS 来存储这些数据，采用带 SSD 存储的EC2 instance
 
 * 也可以使用云中的高性能的 NAS 存储，通过 NFS 方式访问数据



AWS HPC 方案的优势：


