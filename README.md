# Revolution5

## **#1 신용위험 분석 데이터**

<pre><code>- id = A unique LC assigned ID for the loan listing.
- member_id = A unique LC assigned Id for the borrower member.
- loan_amnt = The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
- funded_amnt = The total amount committed to that loan at that point in time.
- funded_amnt_inv = The total amount committed by investors for that loan at that point in time.
- term = The number of payments on the loan. Values are in months and can be either 36 or 60.
- int_rate = Interest Rate on the loan
- installment = The monthly payment owed by the borrower if the loan originates.
- grade = LC assigned loan grade
- sub_grade = LC assigned loan subgrade
- emp_title = The job title supplied by the Borrower when applying for the loan.*
- emp_length = Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
- home_ownership = The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
- annual_inc = The self-reported annual income provided by the borrower during registration.
- verification_status
- issue_d = The month which the loan was funded
- loan_status = Current status of the loan
- pymnt_plan = Indicates if a payment plan has been put in place for the loan
- url = URL for the LC page with listing data.
- desc = Loan description provided by the borrower
- purpose = A category provided by the borrower for the loan request. 
- title = The loan title provided by the borrower
- zip_code = The first 3 numbers of the zip code provided by the borrower in the loan application.
- addr_state = The state provided by the borrower in the loan application
- dti = A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
- delinq_2yrs = The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years
- earliest_cr_line = The month the borrower's earliest reported credit line was opened
- inq_last_6mths = The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
- mths_since_last_delinq = The number of months since the borrower's last delinquency.
- mths_since_last_record = The number of months since the last public record.
- open_acc = The number of open credit lines in the borrower's credit file.
- pub_rec = Number of derogatory public records
- revol_bal = Total credit revolving balance
- revol_util = Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
- total_acc = The total number of credit lines currently in the borrower's credit file
- initial_list_status = The initial listing status of the loan. Possible values are – W, F
- out_prncp = Remaining outstanding principal for total amount funded
- out_prncp_inv = Remaining outstanding principal for portion of total amount funded by investors
- total_pymnt = Payments received to date for total amount funded
- total_pymnt_inv = Payments received to date for portion of total amount funded by investors
- total_rec_prncp = Principal received to date
- total_rec_int = Interest received to date
- total_rec_late_fee = Late fees received to date
- recoveries = post charge off gross recovery
- collection_recovery_fee = post charge off collection fee
- last_pymnt_d = Last month payment was received
- last_pymnt_amnt = Last total payment amount received
- next_pymnt_d = Next scheduled payment date
- last_credit_pull_d = The most recent month LC pulled credit for this loan
- collections_12_mths_ex_med = Number of collections in 12 months excluding medical collections
- mths_since_last_major_derog = Months since most recent 90-day or worse rating
- policy_code = publicly available policy_code=1
new products not publicly available policy_code=2
- application_type = Indicates whether the loan is an individual application or a joint application with two co-borrowers
- annual_inc_joint = The combined self-reported annual income provided by the co-borrowers during registration
- dti_joint = A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income
- verification_status_joint
- acc_now_delinq = The number of accounts on which the borrower is now delinquent.
- tot_coll_amt = Total collection amounts ever owed
- tot_cur_bal = Total current balance of all accounts
- open_acc_6m = Number of open trades in last 6 months
- open_il_6m = Number of currently active installment trades
- open_il_12m = Number of installment accounts opened in past 12 months
- open_il_24m = Number of installment accounts opened in past 24 months
- mths_since_rcnt_il = Months since most recent installment accounts opened
- total_bal_il = Total current balance of all installment accounts
- il_util = Ratio of total current balance to high credit/credit limit on all install acct
- open_rv_12m = Number of revolving trades opened in past 12 months
- open_rv_24m = Number of revolving trades opened in past 24 months
- max_bal_bc = Maximum current balance owed on all revolving accounts
- all_util = Balance to credit limit on all trades
- total_rev_hi_lim
- inq_fi = Number of personal finance inquiries
- total_cu_tl = Number of finance trades
- inq_last_12m = Number of credit inquiries in past 12 months
</code></pre>



#### **데이터 불러오기**
<pre><code>loan = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution5/main/loan.csv')
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

