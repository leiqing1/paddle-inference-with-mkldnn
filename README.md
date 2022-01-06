# paddle-inference-with-mkldnn （python接口）
本repo主要内容：在CPU场景下测试增加mkldnn前后，推理速度变化
1. 首先跑通基本的Paddle inference的python接口推理代码
  参考链接：https://paddle-inference.readthedocs.io/en/latest/quick_start/python_demo.html
2. 为了对比增加mkldnn前后效果，需要修改代码，监控推理速度（数据准备部分耗时、推理耗时、输出耗时）
  具体执行，通过from time import *去监控个模块代码
3.防止一次推理速度不能评测，通过循环跑1000次，去平均值来进行时间监控（具体实现件代码）
4.
