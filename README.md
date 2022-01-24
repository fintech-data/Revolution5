# Revolution5

## **#1 신용위험 분석 데이터**

<pre><code>[1]: id [NaN:0.0%] = A unique LC assigned ID for the loan listing.
[2]: member_id [NaN:0.0%] = A unique LC assigned Id for the borrower member.
[3]: loan_amnt [NaN:0.0%] = The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
[4]: funded_amnt [NaN:0.0%] = The total amount committed to that loan at that point in time.
[5]: funded_amnt_inv [NaN:0.0%] = The total amount committed by investors for that loan at that point in time.
[6]: term [NaN:0.0%] = The number of payments on the loan. Values are in months and can be either 36 or 60.
[7]: int_rate [NaN:0.0%] = Interest Rate on the loan
[8]: installment [NaN:0.0%] = The monthly payment owed by the borrower if the loan originates.
Y1 - [9]: grade [NaN:0.0%] = LC assigned loan grade 
Y2 - [10]: sub_grade [NaN:0.0%] = LC assigned loan subgrade
[11]: emp_title [NaN:5.800000000000001%] = The job title supplied by the Borrower when applying for the loan.*
[12]: emp_length [NaN:5.1%] = Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
[13]: home_ownership [NaN:0.0%] = The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
[14]: annual_inc [NaN:0.0%] = The self-reported annual income provided by the borrower during registration.
[14]:verification_status
[16]: issue_d [NaN:0.0%] = The month which the loan was funded
Y3 - [17]: loan_status [NaN:0.0%] = Current status of the loan
[18]: pymnt_plan [NaN:0.0%] = Indicates if a payment plan has been put in place for the loan
[19]: url [NaN:0.0%] = URL for the LC page with listing data.
[20]: desc [NaN:85.8%] = Loan description provided by the borrower
[21]: purpose [NaN:0.0%] = A category provided by the borrower for the loan request. 
[22]: title [NaN:0.0%] = The loan title provided by the borrower
[23]: zip_code [NaN:0.0%] = The first 3 numbers of the zip code provided by the borrower in the loan application.
[24]: addr_state [NaN:0.0%] = The state provided by the borrower in the loan application
[25]: dti [NaN:0.0%] = A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
[26]: delinq_2yrs [NaN:0.0%] = The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years
[27]: earliest_cr_line [NaN:0.0%] = The month the borrower's earliest reported credit line was opened
[28]: inq_last_6mths [NaN:0.0%] = The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
[29]: mths_since_last_delinq [NaN:51.2%] = The number of months since the borrower's last delinquency.
[30]: mths_since_last_record [NaN:84.6%] = The number of months since the last public record.
[31]: open_acc [NaN:0.0%] = The number of open credit lines in the borrower's credit file.
[32]: pub_rec [NaN:0.0%] = Number of derogatory public records
[33]: revol_bal [NaN:0.0%] = Total credit revolving balance
[34]: revol_util [NaN:0.1%] = Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
[35]: total_acc [NaN:0.0%] = The total number of credit lines currently in the borrower's credit file
[36]: initial_list_status [NaN:0.0%] = The initial listing status of the loan. Possible values are – W, F
[37]: out_prncp [NaN:0.0%] = Remaining outstanding principal for total amount funded
[38]: out_prncp_inv [NaN:0.0%] = Remaining outstanding principal for portion of total amount funded by investors
[39]: total_pymnt [NaN:0.0%] = Payments received to date for total amount funded
[40]: total_pymnt_inv [NaN:0.0%] = Payments received to date for portion of total amount funded by investors
[41]: total_rec_prncp [NaN:0.0%] = Principal received to date
[42]: total_rec_int [NaN:0.0%] = Interest received to date
[43]: total_rec_late_fee [NaN:0.0%] = Late fees received to date
[44]: recoveries [NaN:0.0%] = post charge off gross recovery
[45]: collection_recovery_fee [NaN:0.0%] = post charge off collection fee
[46]: last_pymnt_d [NaN:2.0%] = Last month payment was received
[47]: last_pymnt_amnt [NaN:0.0%] = Last total payment amount received
[48]: next_pymnt_d [NaN:28.499999999999996%] = Next scheduled payment date
[49]: last_credit_pull_d [NaN:0.0%] = The most recent month LC pulled credit for this loan
[50]: collections_12_mths_ex_med [NaN:0.0%] = Number of collections in 12 months excluding medical collections
[51]: mths_since_last_major_derog [NaN:75.0%] = Months since most recent 90-day or worse rating
[52]: policy_code [NaN:0.0%] = publicly available policy_code=1
new products not publicly available policy_code=2
[53]: application_type [NaN:0.0%] = Indicates whether the loan is an individual application or a joint application with two co-borrowers
[54]: annual_inc_joint [NaN:99.9%] = The combined self-reported annual income provided by the co-borrowers during registration
[55]: dti_joint [NaN:99.9%] = A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income
[55]:verification_status_joint
[57]: acc_now_delinq [NaN:0.0%] = The number of accounts on which the borrower is now delinquent.
[58]: tot_coll_amt [NaN:7.9%] = Total collection amounts ever owed
[59]: tot_cur_bal [NaN:7.9%] = Total current balance of all accounts
[60]: open_acc_6m [NaN:97.6%] = Number of open trades in last 6 months
[61]: open_il_6m [NaN:97.6%] = Number of currently active installment trades
[62]: open_il_12m [NaN:97.6%] = Number of installment accounts opened in past 12 months
[63]: open_il_24m [NaN:97.6%] = Number of installment accounts opened in past 24 months
[64]: mths_since_rcnt_il [NaN:97.7%] = Months since most recent installment accounts opened
[65]: total_bal_il [NaN:97.6%] = Total current balance of all installment accounts
[66]: il_util [NaN:97.89999999999999%] = Ratio of total current balance to high credit/credit limit on all install acct
[67]: open_rv_12m [NaN:97.6%] = Number of revolving trades opened in past 12 months
[68]: open_rv_24m [NaN:97.6%] = Number of revolving trades opened in past 24 months
[69]: max_bal_bc [NaN:97.6%] = Maximum current balance owed on all revolving accounts
[70]: all_util [NaN:97.6%] = Balance to credit limit on all trades
[70]:total_rev_hi_lim
[72]: inq_fi [NaN:97.6%] = Number of personal finance inquiries
[73]: total_cu_tl [NaN:97.6%] = Number of finance trades
[74]: inq_last_12m [NaN:97.6%] = Number of credit inquiries in past 12 months
</code></pre>



#### **데이터 불러오기**
<pre><code>loan = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution4/main/loan.csv')
</code></pre>

## **#2 기업 부도 데이터**

<pre><code>Y - Bankrupt? : Class label
X1 - ROA(C) before interest and depreciation before interest: Return On Total Assets(C)
X2 - ROA(A) before interest and % after tax: Return On Total Assets(A)
X3 - ROA(B) before interest and depreciation after tax: Return On Total Assets(B)
X4 - Operating Gross Margin: Gross Profit/Net Sales
X5 - Realized Sales Gross Margin: Realized Gross Profit/Net Sales
X6 - Operating Profit Rate: Operating Income/Net Sales
X7 - Pre-tax net Interest Rate: Pre-Tax Income/Net Sales
X8 - After-tax net Interest Rate: Net Income/Net Sales
X9 - Non-industry income and expenditure/revenue: Net Non-operating Income Ratio
X10 - Continuous interest rate (after tax): Net Income-Exclude Disposal Gain or Loss/Net Sales
X11 - Operating Expense Rate: Operating Expenses/Net Sales
X12 - Research and development expense rate: (Research and Development Expenses)/Net Sales
X13 - Cash flow rate: Cash Flow from Operating/Current Liabilities
X14 - Interest-bearing debt interest rate: Interest-bearing Debt/Equity
X15 - Tax rate (A): Effective Tax Rate
X16 - Net Value Per Share (B): Book Value Per Share(B)
X17 - Net Value Per Share (A): Book Value Per Share(A)
X18 - Net Value Per Share (C): Book Value Per Share(C)
X19 - Persistent EPS in the Last Four Seasons: EPS-Net Income
X20 - Cash Flow Per Share
X21 - Revenue Per Share (Yuan ¥): Sales Per Share
X22 - Operating Profit Per Share (Yuan ¥): Operating Income Per Share
X23 - Per Share Net profit before tax (Yuan ¥): Pretax Income Per Share
X24 - Realized Sales Gross Profit Growth Rate
X25 - Operating Profit Growth Rate: Operating Income Growth
X26 - After-tax Net Profit Growth Rate: Net Income Growth
X27 - Regular Net Profit Growth Rate: Continuing Operating Income after Tax Growth
X28 - Continuous Net Profit Growth Rate: Net Income-Excluding Disposal Gain or Loss Growth
X29 - Total Asset Growth Rate: Total Asset Growth
X30 - Net Value Growth Rate: Total Equity Growth
X31 - Total Asset Return Growth Rate Ratio: Return on Total Asset Growth
X32 - Cash Reinvestment %: Cash Reinvestment Ratio
X33 - Current Ratio
X34 - Quick Ratio: Acid Test
X35 - Interest Expense Ratio: Interest Expenses/Total Revenue
X36 - Total debt/Total net worth: Total Liability/Equity Ratio
X37 - Debt ratio %: Liability/Total Assets
X38 - Net worth/Assets: Equity/Total Assets
X39 - Long-term fund suitability ratio (A): (Long-term Liability+Equity)/Fixed Assets
X40 - Borrowing dependency: Cost of Interest-bearing Debt
X41 - Contingent liabilities/Net worth: Contingent Liability/Equity
X42 - Operating profit/Paid-in capital: Operating Income/Capital
X43 - Net profit before tax/Paid-in capital: Pretax Income/Capital
X44 - Inventory and accounts receivable/Net value: (Inventory+Accounts Receivables)/Equity
X45 - Total Asset Turnover
X46 - Accounts Receivable Turnover
X47 - Average Collection Days: Days Receivable Outstanding
X48 - Inventory Turnover Rate (times)
X49 - Fixed Assets Turnover Frequency
X50 - Net Worth Turnover Rate (times): Equity Turnover
X51 - Revenue per person: Sales Per Employee
X52 - Operating profit per person: Operation Income Per Employee
X53 - Allocation rate per person: Fixed Assets Per Employee
X54 - Working Capital to Total Assets
X55 - Quick Assets/Total Assets
X56 - Current Assets/Total Assets
X57 - Cash/Total Assets
X58 - Quick Assets/Current Liability
X59 - Cash/Current Liability
X60 - Current Liability to Assets
X61 - Operating Funds to Liability
X62 - Inventory/Working Capital
X63 - Inventory/Current Liability
X64 - Current Liabilities/Liability
X65 - Working Capital/Equity
X66 - Current Liabilities/Equity
X67 - Long-term Liability to Current Assets
X68 - Retained Earnings to Total Assets
X69 - Total income/Total expense
X70 - Total expense/Assets
X71 - Current Asset Turnover Rate: Current Assets to Sales
X72 - Quick Asset Turnover Rate: Quick Assets to Sales
X73 - Working capitcal Turnover Rate: Working Capital to Sales
X74 - Cash Turnover Rate: Cash to Sales
X75 - Cash Flow to Sales
X76 - Fixed Assets to Assets
X77 - Current Liability to Liability
X78 - Current Liability to Equity
X79 - Equity to Long-term Liability
X80 - Cash Flow to Total Assets
X81 - Cash Flow to Liability
X82 - CFO to Assets
X83 - Cash Flow to Equity
X84 - Current Liability to Current Assets
X85 - Liability-Assets Flag: 1 if Total Liability exceeds Total Assets, 0 otherwise
X86 - Net Income to Total Assets
X87 - Total assets to GNP price
X88 - No-credit Interval
X89 - Gross Profit to Sales
X90 - Net Income to Stockholder's Equity
X91 - Liability to Equity
X92 - Degree of Financial Leverage (DFL)
X93 - Interest Coverage Ratio (Interest expense to EBIT)
X94 - Net Income Flag: 1 if Net Income is Negative for the last two years, 0 otherwise
X95 - Equity to Liability
</code></pre>

#### **데이터 불러오기**
<pre><code>bankruptcy = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution5/main/data/company_bankruptcy.csv')
</code></pre>

