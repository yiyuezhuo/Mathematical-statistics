# 一些函数的近似表达

## gamma函数

stirling公式，误差太大，放弃

Gergő Nemes近似式 不错，可以直接计算（下面可以直接计算表示没有显示循环和递归和级数/连分数截断）

## beta函数

用近似gamma函数直接表达 虽然会造成误差累积

## 误差函数erf

使用一个可以直接计算的近似式 2.5*10^-4 精度

## 标准正态分布cdf

0处泰勒展开级数            

分部积分法导出的级数  带阶乘的级数数值上都没用

分部积分法导出的级数导出的连分数  

用近似误差函数表示  用的这个，虽然有累计误差

## 标准正态分布分位数(ppf)

山内近似公式 精度4.9*10^-4 形式简单

## 一般正态分布cdf与ppf

利用标准正态分布相应近似式变换而来

## beta分布cdf

分部积分法导出的级数

分部积分法导出的级数的连分数  在靠近0处有数值问题

递归关系  精确但定义域受限，用于资瓷t分布和F分布

## beta分布ppf

beta分布cdf上用二分法(因为限制在[0,1]，性能不算太糟)

## 卡方分布cdf

递归关系 

## 卡方分布分位数

n=1,2特值加两个可以直接计算的近似式（用上估计的标准正态分布ppf）

## t分布cdf  

利用t分布cdf与beta分布cdf关系  虽然累积误差但这里只需要使用beta分布递归情况并不太糟

## t分布ppf

特例+近似式 除了两边的极限情况基本可以接受

## F分布cdf

利用F分布cdf于beta分布cdf关系

## F分布ppf

特例+近似式 疑似仍有数值问题

递归关系精确计算 （一般可以利用gamma分布，不过那个也没什么好的算法，只是个关系而已）


