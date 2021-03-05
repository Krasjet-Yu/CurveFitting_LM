# CurveFitting_LM
# 说明

## 代码说明

app 文件夹下实现了曲线问题的定义，残差计算，数据产生，以及主程序。

backend 文件夹下主要是最小二乘问题求解的一些函数定义。

样例代码给出了使用LM算法估计曲线y = exp（ax^2 + bx + c）参数a，b，c的完整过程
1. 绘制代码中LM阻尼因子u随着迭代变化的曲线图
2. 将曲线函数改成y = ax^2 + b + c, 修改代码中残差计算，雅克比计算等函数，完成曲线参数估计。
3. 实现其他更优秀的阻尼因子策略，并给出实验对比。策略参考论文The Levecbery-Marquardt method for nonlinear least squares curve-fitting problems.

### 代码编译

``` c++
cd CurveFitting_LM
mkdir build
cd build
cmake ..
make -j4    
```

代码运行

```c++
./CurveFitting_LM
```
