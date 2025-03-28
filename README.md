# Optimizing the Output from the Generalized Cobb-Douglas Production Function with Cost Constraints

## Contents

1. [Introduction](#introduction)
2. [Problem Statement](#problem-statement)
3. [Objectives](#objectives)
4. [Results](#results)
5. [Conclusion and Recommendations](#conclusion-and-recommendations)

---

## Introduction

- In economics, a production function relates the physical output of a production process to physical inputs or factors of production.
- It is a mathematical function that relates the amount of output that can be obtained from a given number of inputs.
- The production function could be expressed in a general form such as $Q=f(x_1, x_2, \cdot, x_n)$, where $Q$ denotes the output of the firm, and $x_1, x_2, \cdots, x_n$ are the values of inputs.
- Apart from production function, another important concept in economics is the economic cost. 
- If a firm is producing output $Q$ based on $n$ inputs $x_1, x_2, \cdots, x_n$, where the prices of inputs are $r_1, r_2, \cdots, r_n$ then the total cost of the firm is given by:

  $$C=r_1x_1+r_2x_2+\cdots +r_nx_n$$

 **Example**:
 Cobb-Douglass production function, Constant Elasticity of Substitution production function, Linear production function, etc.

### Why production functions?

- The production function is the central part of productiontheory, and there is theoretical interest in its estimates.
- Economists are often involved in describing activity at the level of a firm, an industry, or the economy as a whole through the production function approach
- he production function also gives information about increasing or decreasing returns to scale and the marginal products of labor and capital.


## Problem Statement

- A most familiar empirical production function found out by statistical methods is the Cobb-Douglas production function.
- When there are two inputs $K$ and $L$, the Cobb-Douglass production function has the form: $Q=AL^{\alpha}K^{\beta}$,  with $Q$ as the  output, $L$ as the quantity of labour employed, $K$ as the quantity of capital employed, and $A, \alpha$ and $\beta$ are positive constants.
- In its general form, where more than two inputs are needed  

$$Q=A \prod_{i=1}^n L_{i}^{\alpha_i}, \quad L=\left(L_1, L_2, \cdots,  L_n\right)$$

- In this final year project, we consider  a firm that buys four inputs $K, L, R$, and $M$, for its production output $Q$ over a period of 12 months.
- The set data representing these variables is available. The Cobb-Douglass production of this firm is given by:

$$Q(K,L,R,M) = AK^{\alpha}L^{\beta}R^{\gamma}M^{\eta}$$

- Assuming that the firm has the amount $C$, which maybe used to buy the four inputs, it follows that we must have the equality $r_1K+r_2L+r_3R+r_4M=C$.
- Using the estimated parameters $\hat{\alpha}, \hat{\beta}, \hat{\gamma}, \hat{\eta}$,  the second problem considered is to optimize the production under this constraint of available cost. Mathematically, we consider the problem:

$$
\begin{array}{ccc}
\text{Optimize} & Q(K,L,R,M) = A K^{\hat{\alpha}} L^{\hat{\beta}} R^{\hat{\gamma}} M^{\hat{\eta}} \\
\text{Subject to} & r_1 K + r_2 L + r_3 R + r_4 M = C.
\end{array}
$$

- Given the amount  $Q_0$ of the production of that a firm want to get, and the price of each unit of the outputs $K,L,R,M$ and the available amount of money $C$, we want to determine an optimal combination of these inputs:

  $$
\begin{array}{ccc}
\text{Optimize} & Q(K,L,R,M) = A K^{\hat{\alpha}} L^{\hat{\beta}} R^{\hat{\gamma}} M^{\hat{\eta}} \\
\text{Subject to} & r_1 K + r_2 L + r_3 R + r_4 M = C.
\end{array}
$$

Mathematically, the problem to solve is the following:

$$
\begin{array}{ccc}
\text{Optimize} & r_1K + r_2L + r_3R + r_4M = C \\
\text{Subject to} & A K^{\hat{\alpha}} L^{\hat{\beta}} R^{\hat{\gamma}} M^{\hat{\eta}} = Q_0.
\end{array}
$$

- The problems are solved by using the method of Lagrange multiplies.


## Objectives

- **Primary Objective**: o optimize the output from the generalized Cobb-Douglass production function in a given company where more than two inputs are available
while accounting for cost linear constraints satisfied by those inputs.
- **Secondary Objectives**:
    - To estimate the parameters of the generalized Cobb-Douglass production function in a firm with more than two inputs.
    - To determine how much output to produce from the Cobb-Douglas production function for a given amount of inputs.
    - To know the maximum output from the Cobb-Douglass production function, and what combination of inputs to be used given the price of inputs.
 
**Example of a Cobb-Douglass production function**:

- Here's an example of a production function: $Q = K^{0.3} \cdot L^{0.7}$.
- Here, $Q$ represents the total output, $K$ represents the amount of capital used in production, and $L$ represents the amount of labor used in production. 
- The exponents $0.3$ and $0.7$ represent the elasticity of output with respect to capital and labor, respectively.
- If we have $10$ units of capital and $20$ units of labor, we can calculate the total output as follows:
  
$$Q =  10^{0.3} \cdot 20^{0.7}=16.245$$


## Results

### Estimating the parameters in the Cobb-Douglass production function

- We consider a firm which uses the Cobb-Douglass production functions with four inputs $K,L,M$ and $N$.
- The production $Q$ and the units of inputs used over a period of 12 months are presented in the following table.

| Months |   Q  |  K  |  L  |  M  |  N  |
|--------|----:|---:|---:|---:|---:|
| Jan    | 240 | 25 | 24 | 91 | 100 |
| Feb    | 236 | 31 | 21 | 90 |  95 |
| Mar    | 270 | 45 | 24 | 88 | 110 |
| Apr    | 274 | 60 | 25 | 87 |  88 |
| May    | 301 | 65 | 25 | 91 |  94 |
| Jun    | 316 | 72 | 26 | 94 |  99 |
| Jul    | 300 | 80 | 25 | 87 |  97 |
| Aug    | 296 | 84 | 25 | 86 |  96 |
| Sep    | 267 | 75 | 24 | 88 | 110 |
| Oct    | 276 | 60 | 25 | 91 | 105 |
| Nov    | 288 | 50 | 25 | 90 | 100 |
| Dec    | 261 | 38 | 23 | 89 |  98 |

- Using the concepts from Multiple linear regression, we estimate the parameters of the Cobb-Douglass  Production function \ref{Albert} of this firm:

$$Q = 0.768 \cdot K^{0.147} \cdot L^{0.521} \cdot M^{0.763} \cdot N^{0.044}$$

- Since $\alpha + \beta + \gamma + \eta=0.147172253 + 0.520665159 + 0.762692634 + 0.044302849 = 1.474832894  > 1$, it follows that we have increasing returns to scale.
- This means that the output increases in a greater proportion than the increase in all inputs.
- Since the efficient parameter $A = 0.768$ it follows  that the inputs used in the production process are being used with an efficiency of $76.8\%$ of their maximum potential.

### Optimizing the outputs from the Cobb-Douglass production function

- The firm with the data above wants to buy the four inputs $K, L, M$, and $N$ at a per unit price of $\$ 50, \$ 30, \$ 25$ and $ \$ 20$, respectively, and operate with the production function $Q$.
- The problem is to know the optimal output it can make for a total cost of $ \$ 30,000$.  Mathematically, the problem to solve is the following:

$$
\begin{eqnarray}
\begin{array}{ccc}
\text{Optimize} &Q= 0.768 \cdot K^{0.147} \cdot L^{0.521} \cdot M^{0.763} \cdot N^{0.044}\\
\text{Subject to } &  50K + 30L +25M + 20N=30,000 
\end{array}
\end{eqnarray}
$$

- Using the method of Lagrange multipliers we obtain the following value
$K = 59.7966102, L = 353.220339, M = 620.745763,\text{ and } N = 44.7457627$
- Testing the nature of this point, we conclude that the point gives the maximum output for the firm.  Hence the maximum  of the firm under the given constraint is given by:

$$Q_{\max}(K,L,M,N) = 4,760.91877869938 $$

###  Optimum combination of inputs for a determined output

- We consider the same firm with the same production function, where four inputs are required, with the production function.
  
$$Q = 0.768 \cdot K^{0.147} \cdot L^{0.521} \cdot M^{0.763} \cdot N^{0.044}  $$

- The inputs prices per unit are the same as in the previous section. We assume that the company want an output of $1,200$ units, and the question is to find the optimum way of producing these units.
- The mathematical problem to solve is the following:

$$
\begin{eqnarray}
\begin{array}{ccc}
\text{Optimize } & 50K + 30L +25M + 20N\\
\text{Subject to } &  0.768 \cdot K^{0.147} \cdot L^{0.521} \cdot M^{0.763} \cdot N^{0.044} = 1,200 
\end{array}
\end{eqnarray}
$$

- The stationary point is given by: $K = 23.49131857, L = 138.76391129, M = 243.86225946, N = 17.57853771$
- Testing the nature of this point, we conclude that the point gives the minimum. Thus the values for $K, L, M, N$ determine the the minimum point.
- Accordingly, the cheapest cost level for producing this output will therefore be $50(23.49131857)+ 30(138.76391129) +25(243.86225946) + 20(17.57853771)= \$ 11,785.6105079$

## Conclusion and Recommendations

### Conclusion
- In this work we have used the method of  Lagrange multipliers to solve problem  related to optimization of production function under a set of cost constraints.
- We have estimated the parameters of the Cobb-Douglass production function in a firm with four inputs, by using the data on a period of 12 months.
- We have optimized the output from the Cobb-Douglass production function under one linear constraint.
- We have determined the optimal combination of inputs given the amount of units in the outputs the firm want to produce.

### Recommendations

- Future research could use real-world data to validate the results and provide more practical insights.
- Future research could compare the Generalized Cobb-Douglass Production Function with other production functions such as the CES Production Function to determine the best fit for different industries and situations.

  $$\frac{\partial^2 G}{\partial K^2}  = \lambda \left(0.096630976K^{-1.853}L^{0.521}M^{0.763}N^{0.044}\right)$$
  
 $$\frac{\partial^2 G}{\partial K \partial L}  = \lambda \left(-0.056418048K^{-0.853}L^{-0.479}M^{0.763}N^{0.044}\right) $$
 
$$\frac{\partial^2 G}{\partial K \partial M}  = \lambda \left(-0.086139648K^{-0.853}L^{0.521}M^{-0.237}N^{0.044}\right)$$

 $$\frac{\partial^2 G}{\partial K \partial N}   = \lambda \left(-0.004967424K^{-0.853}L^{0.521}M^{0.763}N^{-0.956}\right)$$
 
$$\frac{\partial^2 G}{\partial L^2}   =  \lambda \left(0.191661312K^{0.147}L^{-1.479}M^{0.763}N^{0.044}\right)$$

$$\frac{\partial^2 G}{\partial L \partial M}   = \lambda \left(-0.305297664K^{0.147}L^{-0.479}M^{-0.237}N^{0.044}\right)$$

$$\frac{\partial^2 Q}{\partial L \partial N}   = \lambda \left(-0.017605632K^{0.147}L^{-0.479}M^{0.763}N^{-0.956}\right)$$

$$\frac{\partial^2 G}{\partial M^2}   =  \lambda \left(0.138878208K^{0.147}L^{0.521}M^{-1.237}N^{0.044}\right)$$

$$\frac{\partial^2 G}{\partial M \partial N}  = \lambda \left(-0.025783296K^{0.147}L^{0.521}M^{-0.237}N^{-0.956}\right)$$

$$\frac{\partial^2 G}{\partial N^2} = \lambda \left(0.032305152K^{0.147}L^{0.521}M^{0.763}N^{-1.956}\right)$$

Thus the matrix $\pmb{W}$ which is symmetric is given by

$$\pmb{W} = \begin{bmatrix}
\dfrac{\partial^2 G}{\partial K^2} & \dfrac{\partial^2 G}{\partial K \partial L} & \dfrac{\partial^2 G}{\partial K \partial M} & \dfrac{\partial^2 G}{\partial K \partial N}\\\\
\dfrac{\partial^2 G}{\partial L \partial K} & \dfrac{\partial^2 G}{\partial L^2} & \dfrac{\partial^2 G}{\partial L \partial M} & \dfrac{\partial^2 G}{\partial L \partial N}\\\\
\dfrac{\partial^2 G}{\partial M \partial K} & \dfrac{\partial^2 G}{\partial M \partial L} &   \dfrac{\partial^2 G}{\partial M^2}  & \dfrac{\partial^2 G}{\partial M \partial N}\\\\
\dfrac{\partial^2 G}{\partial N \partial K} & \dfrac{\partial^2 G}{\partial N \partial L} & \dfrac{\partial^2 G}{\partial N \partial M} & \dfrac{\partial^2 G}{\partial N^2} 
\end{bmatrix}$$

$$=\begin{bmatrix}                1.82179884	& -0.180066521	& -0.156440771 &	-0.00051321\\\\
-0.180066521 &	0.103557185	& -0.093864463	& -0.07509157\\\\
-0.156440771 &	-0.093864463 &	0.024296503	 & -0.062576309\\\\
-0.00051321 &	-0.07509157	& -0.062576309 &	1.087690018
\end{bmatrix}$$




