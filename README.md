# Modern-Portfolio-Theory-Markowitz-Model-
Explored Modern Portfolio Theory (Markowitz Model), focusing on diversification, mean-variance analysis, the efficient frontier, Sharpe ratio, and the Capital Allocation Line (CAL) to build optimal portfolios and balance risk with expected return.

**Modern Portfolio Theory :** 
* It was first formulated by **Harry Markowitz** back in 1952;
* He was later with the Nobel prize in economics.
* It is a **portfolio optimization** model.
* It assists in the selection of **the most efficient portfolio** by considering various possible portfolios of the given securities based on expected return (mean) and risk (variance).

* The model relies heavily on **historical data**, historical mean performance is assumed to be the best estimator for future (expected) performance.

* **What is the main idea behind Markowitz-Model ?**
  We may  **combine multiple assets(stocks)** in order to reduce risk as much as possible. This is called diverzification.

if we invest all of our money into **a single stock** then we take a huge risk because stocks are **volatile**. We do not know for certain whether the **S(t) stock prioce** will rise or fall. 

**Log Returns Formulation :**
* In financial mathematics, the continuously compounded return (log return) is given by:

$$
r_t = \ln\left(\frac{P_{t+1}}{P_t}\right) = \ln P_{t+1} - \ln P_t
$$

Where:

* 𝑟t : is the log return.
* S(t) : is the asset price at time t.

​In Modern Portfolio Theory, the percentage return \( R_p \) on a linear portfolio is a weighted sum of the returns on its constituent assets:

$$
R_p = \sum_{i=1}^k w_i r_i
$$

where:
\begin{itemize}
    \item $w_i$ is the weight of asset $i$ in the portfolio,
    \item $r_i$ is the return on asset $i$.
\end{itemize}

It is convenient to write this in matrix form.  
Let $r$ denote the $(k \times 1)$ vector of asset returns and $w$ the $(k \times 1)$ vector of portfolio weights:

$$
w = (w_1, w_2, \dots, w_k)^\top, \quad r = (r_1, r_2, \dots, r_k)^\top
$$

Then the portfolio return can be written compactly as:

$$
R_p = w^\top r
$$


The risk of a portfolio can be measured by its variance, using the properties of the variance operator:



In matrix notation, if $\(\Sigma\)$ is the $\(k \times k\)$ covariance matrix of asset returns:

$$
\mathrm{Var}(R_p) = w^\top \Sigma\, w
$$

The portfolio standard deviation is:

$$
\sigma_p = \sqrt{w^\top \Sigma\, w}
$$


* **Assumptions of the Markowitz-Model :**
1) **Returns are normally distributed :** the returns of the stocks are **normally distributed** with **µ mean** and **σ Standard Deviation**.
2) **Investors are Risk-Averse** investors will take on **more risk** if they are expecting **more return**.

* If there is a low risk (bonds) the return is low as well, with the higher isk (stocks) the returns are usually higher.
* **So the efficient Portfolio is the Portfolio that has the highest reward for a given Level of Risk or the Lowest Risk for a Given Return !**


We studied key concepts including:

* **Diversification**: Reducing risk by investing in a variety of assets that do not perfectly correlate with each other.
* **Mean and Variance**: Measuring the expected return (mean) and risk (variance or standard deviation) of asset returns.
* **Efficient Frontier and Sharpe Ratio**: Identifying the set of optimal portfolios that offer the highest expected return for a given level of risk, and using the Sharpe ratio to evaluate performance.
* **Capital Allocation Line (CAL)**: Combining a risk-free asset with a portfolio of risky assets to find the best risk-return trade-off.

In practice, we implemented Python code to:

* Download historical stock data (2012–2025) using the *yfinance* library for a selected group of companies: AAPL, WMT, TSLA, GE, AMZN, DB.
* Visualize the data using an interactive plot (via *plotly*), showing the closing prices of these stocks over time.

This sets the groundwork for further analysis, such as computing returns, portfolio optimization, plotting the efficient frontier, and calculating the Sharpe ratio.


## This chart shows the evolution of closing prices for six major stocks (AAPL, WMT, TSLA, GE, AMZN, DB) from 2012 to 2025.
<img width="1156" height="525" alt="newplot" src="https://github.com/user-attachments/assets/82b96279-9a28-49ea-899b-547abca24a97" />






