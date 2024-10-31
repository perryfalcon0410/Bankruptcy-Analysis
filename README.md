# Company Bankruptcy Analysis

## a. Goals of the Project:
The primary goal of this project is to analyze historical company bankruptcy data to:
1. **Identify key factors** that contribute to financial distress.
2. **Predict bankruptcy risks** using machine learning models.
3. **Provide recommendations** for businesses and investors to mitigate risks.
4. **Offer insights** for policymakers to design effective financial regulations.

## b. Data Sources Used:
The dataset used in this project was sourced from the **Taiwan Economic Journal**. It includes data on company bankruptcies from 1999 to 2009, influenced by the Dotcom Bubble and the Global Financial Crisis.
['Dataset link'](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction)

## c. Data Overview:
### Data Structure:
The dataset includes the following columns:
- **Company Name**: The name of the company.
- **Industry**: The industry to which the company belongs.
- **Financial Indicators**: Metrics such as total assets, liabilities, working capital, and revenue, etc.
- **Bankruptcy Status**: Binary column indicating whether a company went bankrupt (1) or not (0).
- **Date Range**: The data covers a 10-year span from 1999 to 2009.

### Detailed Data Structure:

#### Class Label:
- **Y**: Bankrupt?
#### Features:
- **X1**: ROA(C) before interest and depreciation before interest: Return On Total Assets (C)
- **X2**: ROA(A) before interest and % after tax: Return On Total Assets (A)
- **X3**: ROA(B) before interest and depreciation after tax: Return On Total Assets (B)
- **X4**: Operating Gross Margin: Gross Profit / Net Sales
- **X5**: Realized Sales Gross Margin: Realized Gross Profit / Net Sales
- **X6**: Operating Profit Rate: Operating Income / Net Sales
- **X7**: Pre-tax net Interest Rate: Pre-Tax Income / Net Sales
- **X8**: After-tax net Interest Rate: Net Income / Net Sales
- **X9**: Non-industry income and expenditure/revenue: Net Non-operating Income Ratio
- **X10**: Continuous interest rate (after tax): (Net Income - Exclude Disposal Gain or Loss) / Net Sales
- **X11**: Operating Expense Rate: Operating Expenses / Net Sales
- **X12**: Research and development expense rate: Research and Development Expenses / Net Sales
- **X13**: Cash flow rate: Cash Flow from Operating / Current Liabilities
- **X14**: Interest-bearing debt interest rate: Interest-bearing Debt / Equity
- **X15**: Tax rate (A): Effective Tax Rate
- **X16**: Net Value Per Share (B): Book Value Per Share (B)
- **X17**: Net Value Per Share (A): Book Value Per Share (A)
- **X18**: Net Value Per Share (C): Book Value Per Share (C)
- **X19**: Persistent EPS in the Last Four Seasons: EPS - Net Income
- **X20**: Cash Flow Per Share
- **X21**: Revenue Per Share (Yuan ¥): Sales Per Share
- **X22**: Operating Profit Per Share (Yuan ¥): Operating Income Per Share
- **X23**: Per Share Net profit before tax (Yuan ¥): Pretax Income Per Share
- **X24**: Realized Sales Gross Profit Growth Rate
- **X25**: Operating Profit Growth Rate: Operating Income Growth
- **X26**: After-tax Net Profit Growth Rate: Net Income Growth
- **X27**: Regular Net Profit Growth Rate: Continuing Operating Income after Tax Growth
- **X28**: Continuous Net Profit Growth Rate: Net Income - Excluding Disposal Gain or Loss Growth
- **X29**: Total Asset Growth Rate: Total Asset Growth
- **X30**: Net Value Growth Rate: Total Equity Growth
- **X31**: Total Asset Return Growth Rate Ratio: Return on Total Asset Growth
- **X32**: Cash Reinvestment %: Cash Reinvestment Ratio
- **X33**: Current Ratio
- **X34**: Quick Ratio: Acid Test
- **X35**: Interest Expense Ratio: Interest Expenses / Total Revenue
- **X36**: Total debt / Total net worth: Total Liability / Equity Ratio
- **X37**: Debt ratio %: Liability / Total Assets
- **X38**: Net worth / Assets: Equity / Total Assets
- **X39**: Long-term fund suitability ratio (A): (Long-term Liability + Equity) / Fixed Assets
- **X40**: Borrowing dependency: Cost of Interest-bearing Debt
- **X41**: Contingent liabilities / Net worth: Contingent Liability / Equity
- **X42**: Operating profit / Paid-in capital: Operating Income / Capital
- **X43**: Net profit before tax / Paid-in capital: Pretax Income / Capital
- **X44**: Inventory and accounts receivable / Net value: (Inventory + Accounts Receivables) / Equity
- **X45**: Total Asset Turnover
- **X46**: Accounts Receivable Turnover
- **X47**: Average Collection Days: Days Receivable Outstanding
- **X48**: Inventory Turnover Rate (times)
- **X49**: Fixed Assets Turnover Frequency
- **X50**: Net Worth Turnover Rate (times): Equity Turnover
- **X51**: Revenue per person: Sales Per Employee
- **X52**: Operating profit per person: Operating Income Per Employee
- **X53**: Allocation rate per person: Fixed Assets Per Employee
- **X54**: Working Capital to Total Assets
- **X55**: Quick Assets / Total Assets
- **X56**: Current Assets / Total Assets
- **X57**: Cash / Total Assets
- **X58**: Quick Assets / Current Liability
- **X59**: Cash / Current Liability
- **X60**: Current Liability to Assets
- **X61**: Operating Funds to Liability
- **X62**: Inventory / Working Capital
- **X63**: Inventory / Current Liability
- **X64**: Current Liabilities / Liability
- **X65**: Working Capital / Equity
- **X66**: Current Liabilities / Equity
- **X67**: Long-term Liability to Current Assets
- **X68**: Retained Earnings to Total Assets
- **X69**: Total income / Total expense
- **X70**: Total expense / Assets
- **X71**: Current Asset Turnover Rate: Current Assets to Sales
- **X72**: Quick Asset Turnover Rate: Quick Assets to Sales
- **X73**: Working Capital Turnover Rate: Working Capital to Sales
- **X74**: Cash Turnover Rate: Cash to Sales
- **X75**: Cash Flow to Sales
- **X76**: Fixed Assets to Assets
- **X77**: Current Liability to Liability
- **X78**: Current Liability to Equity
- **X79**: Equity to Long-term Liability
- **X80**: Cash Flow to Total Assets
- **X81**: Cash Flow to Liability
- **X82**: CFO to Assets
- **X83**: Cash Flow to Equity
- **X84**: Current Liability to Current Assets
- **X85**: Liability-Assets Flag: 1 if Total Liability exceeds Total Assets, 0 otherwise
- **X86**: Net Income to Total Assets
- **X87**: Total assets to GNP price
- **X88**: No-credit Interval
- **X89**: Gross Profit to Sales
- **X90**: Net Income to Stockholder's Equity
- **X91**: Liability to Equity
- **X92**: Degree of Financial Leverage (DFL)
- **X93**: Interest Coverage Ratio (Interest expense to EBIT)
- **X94**: Net Income Flag: 1 if Net Income is Negative for the last two years, 0 otherwise
- **X95**: Equity to Liability

### Data Description:
The dataset provides financial data for companies, and the target variable is whether a company declared bankruptcy during the given time frame. The data is useful for understanding the financial characteristics of failing companies.

## d. Tools and Technologies Applied:
The following tools and technologies were used in the analysis:
- **Programming Language**: Python
- **Libraries**:
  - `pandas`: For data manipulation and analysis.
  - `numpy`: For numerical operations.
  - `matplotlib` & `seaborn`: For data visualization.
  - `scikit-learn`: For machine learning and predictive modeling.
  - `ppscore`: For feature importance scoring.
  - `lazypredict`: For rapid prototyping of machine learning models.

## e. Key Insights Discovered:
1. **Key Financial Metrics**: Features such as working capital, total liabilities, and operating expenses are highly correlated with bankruptcy risk.
2. **Industry Vulnerability**: Certain industries, such as technology and retail, showed higher bankruptcy rates, especially during the Dotcom Bubble and Financial Crisis.
3. **Predictive Power**: Financial ratios (liabilities-to-assets, cash flow) are strong predictors of bankruptcy.

## f. Hypotheses Based on Insights:
1. **Companies with higher liabilities relative to assets** are more likely to declare bankruptcy, especially in times of economic downturns.
2. **Industries that rely on rapid technological advancements**, like tech companies, are more susceptible to bankruptcy in times of economic bubbles (e.g., Dotcom Bubble).  
3. **Cash flow problems** can serve as an early indicator of bankruptcy, even if a company has substantial assets.

## g. Recommendations Based on Analysis Results:
1. **For Businesses**: Focus on maintaining a healthy balance of assets and liabilities to safeguard against economic downturns. Prioritize improving cash flow management.
2. **For Investors**: Diversify portfolios across industries and carefully monitor companies' financial ratios, especially liabilities-to-assets and working capital trends.
3. **For Policymakers**: Implement financial stress tests in highly volatile industries, such as tech, to pre-emptively identify at-risk companies and intervene where necessary.

## h. Project Details:

For a detailed breakdown of the analysis, please refer to the project notebook available at the following link:

[Bankruptcy_Analysis.ipynb](https://github.com/perryfalcon0410/Bankruptcy-Analysis/blob/main/Bankruptcy_Analysis.ipynb)
