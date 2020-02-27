# Bayesian

## Bayesian Computing in the Statistics and Data Science Curriculum

+ Non-simulation approach:  

  - discrete bayes 

  - conjugate analysis 

  - normal approximation (e.g., to bionomial dist under big n, ~N(np, sqrt(npq)) )

### Logistic Model/Regression and Odds （案例）

+ 从 Odds(事件发生比) 角度理解 Logistic Regression 模型的参数 http://vividfree.github.io/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0/2015/12/13/understanding-logistic-regression-using-odds

+ 这是作为二分类问题的一种映射模型，类比于回归的方式，将各因子线性加权（实数域，决定了为什么选择拟合到 log（Odds））并映射到概率空间中。核心是利用比如梯度下降的方法估计／学习出 加权参数，这个参数的分布，其极值（MAP）直接可以用做以下推演： 给定观察因子的值，用最优参数值代入，即可推演出 该观察现象发生的概率。

+ 贝叶斯分析的非模拟方法基本思路 （non-Simulation approaches to Bayesian computing）

  - 显式离散熟悉的后验概率函数，可以用贝叶斯公式直接计算后验值。
  
  - 显式连续可对参数进行微分的，采用梯度下降法。
  
  - 显式连续不可微分的，可以用离散区间值逐一变化，得到各参数的分布统计估计，但参数一多就有维度陷阱。
  
  - 简易方法是构造 expo family的显式后验，即根据经验给予 熟悉的显式prior。
  
  - 更熟悉的情况可以用大数的正态分布去逼近估计。
  
  - 再往后就是下面的 模拟估计方法：simulation
  
 
+ 贝叶斯分析的模拟方法基本思路 （Simulation-based approaches）
  
  - 虽可直接在显式posterior的函数上直接采样生成simulated samples, 但对于高纬度，复杂模型就不便可行。
  
  - non-conjugate, multi-parameter Bayesian models, exact solutions to th eposterior is analytically unavailable
  
  - Markov chain Monte Carlo
  
    - Gibbs Sampler
    
    - Metropolis-Hastings algorithm
    
    - Hamiltonian Monte Carlo algorithm
    
    
  
  
 
  
  
  
  
  
  
