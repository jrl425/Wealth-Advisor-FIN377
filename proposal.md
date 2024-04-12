# Research Question
## Bigger Question
The broader issue at hand is the increasing responsibility on individuals to manage their retirement savings effectively, amidst a backdrop of volatile markets, unlimited investment options, and complex tax implications. With wealth managers and financial advisors taking 1% of client wealth every year, there is a growing need for tools that can simplify wealth management and retirement preparation, empowering individuals to make informed investment decisions.
## Specific Research Questions
- How can we provide individual investors with a personalized, optimal investment portfolio that aligns with their retirement goals, risk tolerance, and market outlook, without the need for a financial advisor?
- What are the impacts of including non-traditional investment options (such as ESG, cryptocurrency, and real estate) in retirement portfolios, across different levels of risk aversion?
- Can an automated system effectively predict and adjust an individual's investment strategy over time, to maximize retirement savings while minimizing tax implications?
## Type of Project
Our project does not necessarily fit into the usual prediction or analysis models. Instead, it uses a dashboard to run simulations based on what users input, showing them how different investment choices could play out over time in a straightforward and interactive way. Some examples of this would displaying a client's efficient frontier based on the assumptions they put in or showing graphs that display the weights of their portfolio over time between different indexes. Lastly we want to make sure this dashboard is easy to navigate through and easy for a user to learn how to use it by just looking at it for a few seconds. 

# Necessary Data
## Final Dataset Requirements
- Observation Unit: A security. For example, FBTC, VOO, VIGAX, etc. 
- Sample Period: The average expected return, sigma, beta over a timeframe that is long enough to generate an accurate assumption. (5/10 years) This depends on the security.  
- Sample Conditions: Historical data from each security will be in a different dataset and we will calculate the necessary statistics needed for our final dataset and model.
- Necessary Variables: Historical returns, volatility (standard deviation), beta, tax rates, and dividend yields, potentially fees associated with ETFs.
## Data Availability
All historical data this is needed is publicly accessible. We also have current dividend yields and tax rates. Since our dashboard will be for the future, we may have to modify these rates as they will change in the future and the future rates are not available. 
## Data Collection
Additional data will be collected through public financial databases. For example, CRSP, Yahoo Finance, etc..
## Raw Inputs and Storage
Raw inputs will be inputs that the user enters into the dashboard. These inputs will be Age, Retirement age, annual contribution, annual contribution growth rate, current savings / investments, desired retirement income, investment preferences (Crypto, Real Estate, ESG). These will be stored in a dataframe and entered into the model. Similar to the midterm project, we will have an inputs folder that the model reads and the output will be displayed on the dashboard.
## Data Transformation Speculation
Raw market data will be cleaned, normalized, and merged to create a comprehensive dataset. We will also then have to calculate annualized returns and volatility and Beta for each security. This may be difficult as some indexes have not been around for a long time, which brings up the question of how we get an annualized return. For example, Bitcoin ETFs are very new, so it will be difficult to generate an accurate annualized return. To account for this, we will need to research historical data and potentially have to create our own assumptions.

# What the Dashboard Will Look Like
## Summary 
Below are the various inputs and outputs of our wealth advisor dashboard. Enjoy :)
## Inputs
- Age
- Retirement age
- Desired retirement income(Taxed or Pretaxed)
- Current savings/investments
- Annual contribution to savings
- Annual contribution growth rate
- Preference for specific types of investments (e.g., Cryptocurrency, Real Estate, ESG)
- Risk Tolerance(Some sort of scale related to this)
- Market Outlook(Some sort of scale related to what the clients outlook on the market is)
## Outputs
- Portfolio Allocation: Graphs showing the allocation of investments across different asset classes (stocks, bonds, real estate, etc.) over time
- Efficient Frontier Visualization: A plot displaying the efficient frontier based on the user’s risk tolerance and investment preferences, helping them understand the risk/reward trade-off
- Projected Retirement Savings: A graph or series of graphs showing projected growth of the portfolio over time, including contributions and expected returns
- Tax Implications: Visualizations showing potential tax liabilities under different investment scenarios
- Sensitivity Analysis: Charts showing how changes in market conditions or user inputs could impact the portfolio performance
- Comparison Scenarios: Side-by-side comparisons of traditional vs. non-traditional investment strategies (like inclusion of ESG or cryptocurrency) under various market scenarios






