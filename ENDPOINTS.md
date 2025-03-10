<h1 align=center> Endpoints we are providing 💫</h1>

**GET** `/simple_interest_rate`

- Required parameters : `amount_paid`, `principle_amount` and `months`
- Sample output

```py
{
    "Tag": "Simple Interest Rate",
    "Total amount paid": 5000.0,
    "Principle amount": 4500.0,
    "Interest Paid": 500.0,
    "Interest Rate": "11.11111111111111%"
}
```

**GET** `/convexity_duration`

- Required parameters : `rate`,`coupon_rate`,`frequency`,`face_value`,`settlement_date`,`maturity_date`
- Sample output

```py
{
        "Tag": "Convexity Adjusted Duration",
        "Market Rate": 6,
        "Coupon rate":10,
        'Frequency':2
        "Face Value": 100,
        "Settlement Date": '1-1-2020',
        "Maturity Date": '10-10-2024',
        "Convexity Adjusted Duration":3.437535660034277
}
```

**GET** `/payback_period`

- Required parameters : `years_before_recovery`, `unrecovered_cost` and`cash_flow`
- Sample output

```py
{
    "Tag": "Payback period",
    "Years before full recovery": 7,
    "Unrecovered cost at start of the year": 23000.0,
    "Cash flow during the year": 7000.0,
    "Payback period": "10.285714285714285"
}

```

**GET** `/compound_interest`

- Required parameters : `principal_amount`, `intrest_rate` , `years` and `compounding_period`
- Sample output

```py
{
    "Tag": "Compound Intrest Amount",
    "Principle amount": 1000.0,
    "Intrest Rate": 0.05,
    "Time in Years": 2,
    "Compounding Period": 1,
    "Amount after intrest": "1102.5"
}
```

**GET** `/effective_annual_rate`

- Required parameters : `annual_interest_rate`and `compounding_period`
- Sample output

````py
{
  "Tag": "Effective Annual Rate",
  "Annual Intrest Rate": 0.05,
  "Compounding Period": 2,
  "Effective Annual Rate (in percentage)": "5.062499999999992%"

**GET** `/certificate_of_deposit`
+ Required parameters : `principal_amount`, `interest_rate`, `yrs`, and `compounding_per_yr`
+ Sample output
```py
{
    "Tag": "Certificate of Deposit (CD)",
    "Principal amount": 5000.0,
    "Interest Rate": 5.0,
    "Time in Years": 3,
    "Number of Compounding per Year": 1,
    "Certificate of Deposit (CD)": 5788.13,
}
````

**GET** `/roi`

- Required parameters : `current_value_of_investment` and`cost_of_investment`
- Sample output

```py
{
    "Tag": "Return on Investment",
  "Current Value of Investment": 120,
  "Cost of Investment": 100,
  "Return on Investment": "20.0%"
 }
```

**GET** `/compounded_annual_growth_rate`

- Required parameters : `end_investment_value`, `initial_investment_value` and`years`
- Sample output

```py
{
   "Tag":"Compounded Annual Growth Rate",
   "End investment value":100000,
   "Initial investment value":70000,
   "Years":3,
   "Compunded Annual Growth Rate":0.12624788
}
```

**GET** `/asset_portfolio`

- Required parameters : `price_A`, `price_B`, `return_A`, `return_B`, `standard_dev_A`, `standard_dev_B` and `correlation` where A and B refer to the 2 stocks.
- Sample output

```py
{
     "Tag": "Portfolio Variance",
     "Expected Returns": 16.8%,
     "Portfolio Variance": 0.046,
}
```

**GET** `/wacc`

- Required parameters : `firm_equity`, `firm_debt`, `cost_of_equity`, `cost_of_debt`, `corporate_tax_rate`
- Sample output

```py
{
    "Tag": "Weighted Average Cost of Capital(WACC)",
    "Marketvalue of firm's equity" : 30000000,
    "Market value of firm's debt" : 2000000,
    "Cost of equity" : 0.09,
    "Cost of debt" : 0.06,
    "Corporate tax rate" : 0.21,
    "WACC" : 7.3%,
}
```

**GET** `/loan_emi`

- Required parameters : `principle_amount`, `annual_rate` and `months`
- Sample output

```py
{
    "Tag": "Loan Emi",
    "Princiapl amount borrowed": 100000.0,
    "Annual Rate of interest": 7.0,
    "Total number of monthly payments": 120,
    "EMI": "1161.085",
    "Total Amount Payble": "139330.175",
    "Interest amount": "39330.175"
}
```

**GET** `/put-call-parity`

- Required parameters : `call_price`, `put_price` and `strike_price`
- Sample output

```py
{
  "Tag": "Pull Call Parity",
  "Future Price": "800.0",
  "Call Price": "1000.0",
  "Put Price": "500.0",
  "Strike Price": "300.0"
}
```

**GET** `/bep`

- Required parameters : `fixed_cost`, `selling_price` and `variable_cost`
- Sample Output

```py
{
    "Tag" : "Break Even Point (BEP)",
    "Fixed costs" : 2000,
    "Selling price per unit" : 1.50,
    "Variable cost per unit" : 0.40,
    "Break Even Point in units" : 1818.0,
    "Break Even Point in Rupees" : 2727,
}
```

**GET** `\fcff`

- Required parameters : `sales`,`operating_cost`,`depreciation`, `interest`,`tax_rate`,`fcInv` and `wcInv`
- Sample Output (for sales = 200, operating_cost = 20, depreciation = 20, interest = 30, tax_rate = 40%, wcInv = -40 and fcInv = 0

```py
{
    "Tag" : "Free Cash Flow to Firm (FCFF)",
    "Earnings before interest, taxes, depreciation and amortization" : 80.0,
    "Earnings before interest and taxes : " : 60.0 ,
    "Net Income" : 18.0,
    "Free Cash Flow to Firm" : 46.0,
}
```

**GET** `/price_to_earning_ratio`

- Required parameters : `share_price`, `earnings_per_share`
- Sample Output

```py
{
    "Tag" : "Price to Earning ratio",
    "Share price" : 200.0,
    "Earning per share" : 20.0,
    "Price to Earning ratio" : 10.0%,
}
```

**GET** `/dividend_yield_ratio`

- Required parameters : `dividend_per_share`, `share_price`
- Sample Output

```py
{
    "Tag":"Dividend yield ratio",
    "Dividend per share" : 200.0,
    "Share price" : 20.0,
    "Dividend yield ratio" : 10.0%,
}
```

**GET** `/dividend_payout_ratio`

- Required parameters : `dividend_per_share`, `earnings_per_share`
- Sample Output

```py
{
    "Tag":"Dividend payout ratio",
    "Dividend per share" : 200.0,
    "Earnings per share" : 20.0,
    "Dividend payout ratio" : 10.0%,
}
```

**GET** `/debt_to_income_ratio`

- Required parameters : `annual_income`, `total_debt_per_month`
- Sample Output

```py
{
  "Tag": "Debt to income ratio",
  "Annual income": 72000,
  "Total debt per month": 3600,
  "Debt to income ratio per month": "60.0%"
 }
```

**GET** `/fixed_charge_coverage_ratio`

- Required parameters : `earnings_before_interest_taxes`, `fixed_charge_before_tax`,`interest`
- Sample Output

```py
{

    "Tag":"fixed charges coverage ratio",
    "Earnings before interest taxes" : 3000000.0,
    "Fixed charge before tax" : 500000.0,
    "Interest" : 300000.0,
    "Fixed charges coverage ratio" : 4.375%,
}
```

**GET** `/inventory_shrinkage rate`

- Required parameters : `recorded_inventory`, `actual_inventory`
- Sample Output

```py
{
    "Tag":"Inventory shrinkage rate",
    "Recorded Inventory" : 38000,
    "Actual Inventory" : 35000,
    "Invenory Shrinkage Rate" : 0.07894736842105263,
    "Invenory Shrinkage Rate (%)" : 7.894736842105263,
}
```

**GET** `/markup_percentage`

- Required parameters : `price`, `cost`
- Sample Output

```py
{
    "Tag": "Markup Percentage",
    "Price": 50,
    "Cost": 5,
    "Markup Percentage": 900
}
```

**GET** `/sharpe_ratio`

- Required parameters : `portfolio_return`, `risk_free_rate`,`standard_deviation_of_portfolio`
- Sample Output

```py
{

  "Tag": "Sharpe Ratio",
  "Portfolio Return": 25,
  "Risk Free Rate": 5,
  "Standard Deviation of Portfolio": 10,
  "Sharpe Ratio": "2.0"

}
```

**GET** `/Capital_Asset_Pricing_Model`

- Required parameters : `risk_free_interest_rate`, `beta_of_security`,`expected_market_return`
- Sample Output

```py
{

  "Tag": "Capital_Asset_Pricing_Model",
  "risk_free_interest_rate": 2.5"%",
  "beta_of_security": 1.25,
  "expected_market_return": 7.5"%",
  "Capital_Asset_Pricing_Model": "11.9%"

}
```

**GET** `/cost_of_equity`

- Required parameters : `risk_free_rate_of_return`, `Beta`, `market_rate_of_return`
- Sample Output

```py
{
    "Tag": "Cost of Equity",
    "Risk free rate of return": 100,0,
    "Beta": 3.0,
    "Market rate of return ": 200.0,
    "Cost of equity": 400.0%

}
```

**GET** `/cogs`

- Required parameters : `beginning_inventory`,`purchases` and `ending_inventory`
- Sample Output

```py
{
   "Tag": "Cost of Goods Sold",
  "Beginning Inventory": 2000,
  "Purchases during the period": 1500,
  "Ending Inventory": 1000,
  "Cost of Goods Sold(In Rupees)": "2500.0"
}
```

**GET** `/purchasing_power`

- Required parameters : `initial_amount`, `annual_inflation_rate` , `time`
- Sample output

```py
{
     "Tag": "Purchasing Power",
     "Initial Amount": 10000,
     "Annual Inflation Rate": 5,
     "Time in years": 10,
     "Purchasing Power": 6139.13253540759
}
```

**GET** `/monthly_emi`

- Required parameters : `loan_amt`,`interest_rate`,`number_of_installments`
- Sample output

```py
{
    "Tag": "Monthly EMI",
    "Loan Amount": 500000,
    "Interest Rate":8,
    "Number of Installments":24,
    "Total EMI": 22613.645728092295
}
```

**GET** `/doubling_time`

- Required parameters : `r`
- Sample output

```py
{
    "Tag": "Doubling Time",
    "Rate of Interest": 8,
    "Time in years to double the money": 9.006468342000588
}
```

**GET** `/weighted_average`

- Required parameters : `ratio`,`rates`
- Sample output

```py
{
    "Tag": "Weighted Average",
    "Ratio of each investment principal": [0.20, 0.25, 0.35,0.10, 0.10],
    "Rates":[7.5, 8.5, 8, 5, 6],
    "Weighted average : ": 7.525
}
```

**GET** `/ruleof72`

- Required parameters : `rate_of_roi` it should be in percentage only
- Sample output

```py
{
    "Tag": "Rule of 72",
    "Rate of ROI": 5,
    "Time peroid in which investment get double(in years)": "14.4"
}
```

**GET** `/acid-test-ratio`

- Required parameters : `cash`,`marketable_securities`,`accounts_receivable` and `current_liabilities` Note : cash = cash + cash equivalents
- Sample Outuputs

```py
{
    "Tag": "Acid Test Ratio",
    "Cash and Cash Equivalents": 10000,
    "Marketable Securities": 5000,
    "Accounts Receivable": 20000,
    "Current Liabilities": 30000,
    "Acid Test Ratio (Quick Ratio)": "1.17"
}
```

**GET** `/inflation-adjusted-return`

- Required parameters : `beginning_price`, `ending_price`, `dividends`, `beginning_cpi_level` and `ending_cpi_level`
- Sample output

```py
{
    "Tag": "Inflation Adjusted Return",
    "Stock Return": "0.23333333333333334%",
    "Inflation Rate": "0.03%",
    "Inflation Adjusted Return": "19.74%"
}
```

**GET** `/cogr`

- Required parameters : `beginning_value`, `ending_value` and `years`
- Sample output

```py
{
    "Tag": "Coumpound Annual Growth Rate",
    "Beginning Value": 176000,
    "Ending Value": 64900,
    "Compound Annual Growth Rate": "39.5%"
}
```

**GET** `/current_liability_coverage_ratio`

- Required parameters : `net_cash_from_operating_activities`, `total_current_liabilities`, `number_of_liabilities`
- Sample Output

```py
{

  "Tag": "current liability coverage ratio",
  "net_cash_from_operating_activities": 100,
  "total_current_liabilities": 1700,
  "number_of_liabilities": 2,
  "current_liability_coverage_ratio": "0.12"
}
```

**GET** `/levered_beta`

- Required parameters : `unlevered_beta`, `tax_rate`, `debt`,`equity`
- Sample output

```py
{
    "Tag": "Levered Beta",
    "Unlevered Beta": 10.0,
    "Tax rate":0.5,
    "debt": 100.0,
    "Equity": 50.0,
    "Levered Beta":20.0%

}
```

**GET** `/current-ratio`

- Required parameters : `total_current_assets:float` and `total_liabilities`
- Sample output

```py
{
    "Tag": "Current Ratio",
    "Total Current Assets": 100000,
    "Total Liabilities": 125000,
    "Current Ratio": "0.8"
}
```

**GET** `/monthly_payment`

- Required parameters : `principal`, `interest_rate`, `number_of_periods`,`payments_per_period`
- Sample output

```py
{
    "Tag": "Monthly Payment",
    "Principal": 20000,
    "Interest Rate": 16,
    "Number of Periods" : 3,
    "Payments per period": 2,
    "Levered Beta": 160000.0%
    }
```

**GET** `/inventory-turnover-ratio`

- Required parameters : `cost_of_goods_sold`,`beginnning_inventory` and `ending_inventory`
- Sample output

```py
{
    "Tag": "Inventory Turnover Ratio",
    "Cost of Goods Sold": 600000,
    "Inventory Turnover Ratio": "5.0"
}
```

**GET** `/inflation-rate`

- Required parameters : `bigger_year`,`smaller_year` and `base_year`
- Sample output

```py
{
    "Tag": "Inflation Rate",
    "Bigger Year": 2000,
    "Smaller Year": 1000,
    "Base Year": 1000,
    "Inflation Rate": 100
}
```

**GET** `/herfindal_Index`

- Required parameters : `space seperated list of Firms_market_shares`
- Note: Input should be space seperated
- Sample Output

```py
{

  "Tag": "herfindal_Index",
  "Market shares of firm 1" : "40%",
  "Market shares of firm 2" : "30%",
  "Market shares of firm 3" : "15%",
  "Market shares of firm 4" : "15%",
  "Herfindal Index" : 2950
}
```

**GET** `/discount_opex`

- Required parameters : `annual_opex`,`wacc` and `project_lifetime`
- Sample output

```py
{
    "Tag": "Discount OPEX",
    "Annual OPEX": 1000,
    "WACC": 3,
    "project lifetime": 3,
    "Discount opex": 333%
}
```

**GET** `/project_efficiency`

- Required parameters : `annual_production`, `collector_surface`, `dni`
- Sample output

```py
{
    "Tag": "Project efficiency",
    "Annual production": 10000,
    "collector surface": 10,
    "dni": 5,
    "Discount opex": 200%
}
```

**GET** `/real-gdp`

- Required parameters : `nominal_gdp`, `gdp_deflator`
- Sample output

```py
{
  "Tag": "Real GDP",
  "Nominal GDP": 2880,
  "GDP Deflator": 2,
  "Real GDP": 144000
}
```

**GET** `/excess-reserves`

- Required parameters : `deposits`, `reserve_requirement`
- Sample output

```py
{
  "Tag": "Excess Reserves",
  "Deposits": 280,
  "Reserve Requirement": 0.3,
  "Excess Reserves": 196
}
```

**GET** `/discounted_cash_flow`

- Required parameters : `real_feed_in_teriff`, `annual_production`,`wacc`,`project_lifetime`
- Sample output

```py
{
  "Tag": "Discounted cash flow",
  "Real feed in teriff": 1000,
  "annual production": 200,
  "wacc": 10,
  "project lifetime" : 5,
  "discounted cash flow": 20000%,
}
```

**GET** `/gdp-growth-rate`

- Required parameters : `last_year_gdp`, `current_year_gdp`
- Sample output

```py
{
  "Tag": "GDP Growth Rate",
  "Current Year GDP": 3386,
  "Last Year GDP": 2800,
  "GDP Growth Rate": 20.92857142857143
}
```

**GET** `/credit_card_equation`

- Required parameters : `balance`,`monthly_payment`,`daily_interest_rate`
- Sample output

```py
{
   "Tag": "Credit card equation",
    "Balance": 10000,
    "Monthly Payment": 3000,
    "daily interest rate": 2,
    "credit card equation": 3.037283729
}
```

**GET** `/credit_card_payoff`

- Required parameters : `debts`,`monthly_payment`,`interest_rate`,`minimum_payments`
- Sample output

```py
{
   "Tag": "Credit card payoff",
    "debts": [5000,6000,3000],
    "interest rates": [10,15,9],
    "minimum payments":[500,400,300],
    "Monthly payment": 2000,
    "Months":[7,5,8],
    "Interest paid": [194.17,225.0,117.0],
    "Total Payment":[5194.17,6225.0,3117.0]
}
```

**GET** `/future_value_of_ordinary_due`

- Required parameters : `periodic_payment`, `number_of_periods`, `effective_interest_rate`
- Sample Output

```py
{

  "Tag": "future_value_of_ordinary_due",
  "Periodic payment" : "$1000",
  "Number of periods" : "50",
  "Effective interest rate" : "0.6%",
  "Herfindal Index" :  "$58108.22"
}

```

**GET** `/future_value_of_annuity_due`

- Required parameters : `periodic_payment`, `number_of_periods`, `effective_interest_rate`
- Sample Output

```py
{
  "Tag": "future_value_of_annuity_due",
  "Periodic payment" : "$10000",
  "Number of periods" : "10",
  "Effective interest rate" : "5%",
  "Herfindal Index" :  "$132,067.87"
}
```

**GET** `/present_value_of_annuity_due`

- Required parameters : `periodic_payment`, `number_of_periods`, `rate_per_period`
- Sample Output

```py
{
  "Tag": "Present value of annuity due",
  "Periodic payment": 10000,
  "Number of periods": 10,
  "Rate Per Period": 5,
  "PV of Annuity Due": "11999.99980154194"
}
```

**GET** `/compound_annual_growth_rate`

- Required parameters : `ending_value`, `beginning_value`,`number_of_periods`
- Sample Output

```py
{
 "Tag": "compound annual growth rate 1",
 "ending_value": 10000,
 "beginning value": 100,
 "Number of periods": 2,
 "compound annual growth rate": 99%,
}
```

**GET** `/loan-to-value`

- Required parameters : `mortage_value` and `appraised_value`
- Sample Output

```py
{
  "Tag": "Loan to Value (LTV) ratio",
  "Mortage Value": 90000,
  "Appraised Property Value": 100000,
  "Loan to Value ratio": "90.0%"
}
```

**GET** `/retention-ratio`

- Required parameters : `net_income` and `dividends`
- Sample Output

```py
{
  "Tag": "Retention Ratio",
  "Net Income": 580000,
  "Dividends": 23000,
  "Retention Ratio": 0.9603448275862069
}
```

**GET** `/tax_equivalent_yield`

- Required parameters : `tax_free_yield` and `tax_rate`
- Sample Output

```py
{
  "Tag": "Tax Equivalent Yield",
  "Tax Free Yield": 280000,
  "Tax Rate": 0.08,
  "Tax Equivalent Yield": 304347.8260869565
}
```

**GET** `/year-to-year`

- Required parameters : `later_year_value` and `earlier_year_value`
- Sample Output

```py
{
  "Tag": "Year to Year Growth",
  "Year to Year growth": "20.0%"
}
```

**GET** `/future_value_of_annuity`

- Required parameters : `payment_per_periods`,`interest_rate`,`number_of_periods`
- Sample Output

```py
{
   "Tag" : "Future value of annuity",
    "Payments per periods" : 300,
    "interest rate" : 1,
    "number of periods" : 1,
    "future value of annuity" : 300%,
}
```

**GET** `/balloon-balance`

- Required parameters : `present_value`, `payment`,`rate_per_payment`, `number_of_payments`
- Sample Output

```py
{
  "Tag": "Balloon Balance of a Loan",
  "Present Value (Original Balance)": 28268,
  "Payment": 10,
  "Rate per Payment": 2,
  "Number of Payments": 3,
  "Future Value (Balloon Balance)": 763106
}
```

**GET** `/periodic_lease_payment`

- Required parameters : `Asset_value_to_be_financed` and `monthly_lease_interest_rate` and `Number_of_lease_payments_required`
- Sample Output

```py
{
  "Tag": "Periodic lease payment",
  "Asset value to be financed": 20000,
  "Monthly lease interest rate": 0.5%,
  "Number of lease payments required": 36,
  "Pmt": 608.44
}
```

**GET** `/future_sip`

- Required parameters : `interval_investment`,`rate_of_return`,`number_of_payments`
- Sample Output

```py
{
  "Tag": "Future Value of SIP",
  "Investment at every Interval":500 ,
  "Interest": 0.1,
  "Number of Payments": 5,
  "Future Value": 8052.55,
}
```

**GET** `/calculate_pension`

- Required parameters : `monthty_investment_amount`,`no_of_years`,`annuity_rates`,`annuity_purchased`,`yearly_interest_rates`
- Sample output

```py
{
    "Tag": "Calculate Pension",
    "Monthly Investment amount":2000,
    "No. of years": 36,
    "Annuity Purchased":40
    "Annuity Rates": 7,
    "Interest Rate":9,
    "Total Corpus":6759114.79,
    "Lump sum pension":4055468.874,
    "Monthly Pension":15771.27
}
```

**GET** `/inflation`

- Required parameters : `present_amount`,`inflation_rate`,`years`
- Sample Output

```py
{
        "Tag": "Inflated Amount",
        "Present Amount": 1000,
        "Inflation Rate": 4,
        "Time in Years": 5,
        "Future Amount": 1276.28,
}
```

**GET** `/jensens_alpha`

- Required parameters : `return_from_investment`,`return_of_appropriate_market_index`,`risk_free_rate`,`beta`
- Sample Output

```py
{
            "Tag": "Jensen's Alpha",
            "Total return from investment": 100,
            "Return of appropriate market index": 15,
            "Risk free rate": 10,
            "Beta of the portfolio investment w.r.t chosen market index":5 ,
            "Alpha of the return ": 65,
}
```

**GET** `/weighted_average_of_values`

- Required parameters : `Assigned_weight_values`,`data_point_values`
- Note: Input should be space seperated
- Sample Output

```py
{
   "Tag" : "Weighted Average of given values",
    "Assigned weight values" : "2 5 3",
    "data point values" : "10 50 40",
    "weighted_average" : 39
}
```

**GET** `/discounted_payback_period`

- Required parameters : `overflow`,`rate`,`periodic_cash_flow`
- Sample Output

```py
{
  "Tag": "Discounted Payback Period",
  "Initial Investment (Outflow)": 2800,
  "Rate": 2,
  "Periodic Cash Flow": 30000,
  "Discounted Payback Period": 0.18806839455026092
}
```

**GET** `yield-to-maturity`

- Required parameters : `bond_price`, `face_value`, `coupon_rate` and `years_to_maturity`
- Sample output

```py
{
  "Tag": "Yield To Maturity",
  "Face Value": 1000,
  "Years to maturity": 12,
  "Yield to Maturity": "8.76%"
}
```

**GET** `perpetuity-payment`

- Required parameters : `present_value` and `rate`
- Sample output

```py
{
  "Tag": "Perpetuity Payment",
  "Present Value": 1000,
  "Perpetuity Payment": "100.0"
}
```

**GET** `zero_coupoun_bond_value`

- Required parameters : `face_value`, `rate_of_yield` and `time_of_maturity`
- Sample output

```py
{
  "Tag": "Zero Coupon Bond Value",
  "Face Value": 1000,
  "Rate of yield": "6.0%",
  "Zero Coupon Bond Value": 747.26
}
```

**GET** `zero_coupoun_bond_yield`

- Required parameters : `face_value` , `present_value` and `time_of_maturity`
- Sample output

```py
{
  "Tag": "Zero Coupon Bond Effective Yield",
  "Face Value": 1000,
  "Present Value": 742.47,
  "Time to maturity": 10,
  "Zero Coupon Bond Effective Yield": "3.0%"
}
```

**GET** `profitability_index`

- Required parameters : `initial_investment`, `pv_of_future_cash_flows`
- Sample output

```py
{
  "Tag": "Profitability Index",
  "Initial Investment": 28000,
  "PV of Future Cash Flows": 29000,
  "Perpetuity Payment": 1.0357142857142858
}
```

**GET** `/profitability_index2`

- Required parameters : `initial_investment`,`annual_cash_flows`, `discount_rate`
- Note: annual_cash_flows should be space seperated
- Sample Output

```py
{
   "Tag" : "Profitability Index",
    "initial_investment" : 10000,
    "annual_cash_flows" : "5000 4000 3000",
    "discount_rate" : "10%",
    "profitability_index" : 1.003
}
```

**GET** `receivables_turnover_ratio`

- Required parameters : `sales_revenue`, `avg_accounts_receivable`
- Sample output

```py
{
  "Tag": "Receivables Turnover Ratio",
  "Sales Revenue": 202300,
  "Avg Accounts Receivables": 16800,
  "Receivables Turnover Ratio": 12.041666666666666
}
```

**GET** `remainig_balance`

- Required parameters : `regular_payment`, `interest_rate_per_period`,`number_of_payments`,`number_of_payments_done`
- Sample output

```py
{
  "Tag" : "Remainig balance",
  "regular_payment" : 500,
  "interest rate per period" : 3,
  "number of payments" : 36,
  "number of payments done": 26,
  "remaining balance" : 166.6665077
}
```

**GET** `net_present_value`

- Required parameters : `cash_flows`, `discount_rate`,`initial_investment`
- Sample output

```py
{
  "Tag" : "net present value",
  "cash_flows" : "2 4 6 8 10",
  "discount_rate" : 7,
  "initial_investment" : 20,
  "net present value": 3.493
}
```

**GET** `leverage_ratio_income`

- Required parameters : `debt_payments`, `income`,
- Sample output

```py
{
   "Tag": "Leverage Ratio By Income",
   "Debt ": 25687,
   "Income": 676,
   "Leverage Ratio": 37.998520710059172,
}
```

**GET** `leverage_ratio_equity`

- Required parameters : `debt_payments`, `equity`,
- Sample output

```py
{
   "Tag": "Leverage Ratio By Equity",
   "Debt ": 7873,
   "Income": 3938,
   "Leverage Ratio": 1.9992381919756229,
}
```

**GET** `time_period_required_for_growth`

- Required Parameters : `interest_rate`, `growth_factor`
- Sample output

```py
{
 "Tag" : "time period for exponential growth",
 "interest_rate" : 7,
 "growth_factor": 3,
 "time period" : 16.23
}
```

**GET** `preferred-stock-value`

- Required Parameters : `dividend`, `discount_rate`
- Sample output

```py
{
  "Tag": "Preferred stock value",
  "Dividend": 0.25,
  "Discount Rate": 0.005,
  "Preferred Stock Value": 50
}
```

**GET** `/present_value_of_annuity_due`

- Required parameters : `periodic_payment`, `number_of_periods` and `rate_per_period`
- Sample output

```py
{
    "Tag": "Present Value of Annuity Due",
    "Periodic Payment": 5000.0,
    "Number of Periods": 3,
    "Rate Per Period": 10.0,
    "Present Value of Annuity Due": "5495.8677685950415"
}
```

**GET** `/asset_turnover_ratio`

- Required parameters : `net_sales`, `total_asset_beginning` and `total_asset_ending`
- Sample output

=======

```py
{
    "Tag": "Asset Turnover Ratio",
    "Net Sales": 100000.0,
    "Total beginning asset": 20000.0,
    "Total ending asset": 30000.0,
    "Total average asset": 25000.0,
    "Asset Turnover Ratio": "4.0",
}
```

**GET** `/bid-ask-spread`

- Required parameters : `ask_price`, `bid_price`
- Sample output

```py
{
  "Tag": "Bid Ask Spread",
  "Ask Price": 28700,
  "Bid Price": 26200,
  "Bid Ask Spread": 2500
}
```

**GET** `/calculate-period-FV-PV-rate`

- Required parameters : `present_val`, `future_val`,`rate`
- Sample output

```py
{
  "Tag": "Period in years ",
  "Present Value": 5000,
  "Future Vlaue": 6500,
  "Periods": 3.87776389841767
}
```

**GET** `/balloon-loan-payment`

- Required parameters : `principal`, `interest_rate`, `term_years` and `balloon_payment_year`
- Sample output

```py
{
  "Tag": "Balloon loan Payment",
  "Principal": 100000,
  "Interest Rate": 7,
  "Term Years": 30,
  "Balloon Payment Year": 5,
  "Balloon Loan Payment": 94131.5898577919,
}
```

**GET** `/periodic_lease_payment`

- Required parameters : `Asset_value_to_be_financed` and `monthly_lease_interest_rate` and `Number_of_lease_payments_required`
- Sample Output

```py
{
  "Tag": "Monthly lease payment",
  "Asset value to be financed": 20000,
  "Monthly lease interest rate": 0.5%,
  "Number of lease payments required": 36,
  "Pmt": 16.89
}
```

**GET** `/401k`

- Required parameters : `income`, `contribution_percentage`,`current_age`,`age_at_retirement`,`rate_of_return`,`salary_increase_rate`,`withdraw_tax_rate`
- Sample output

```py
{
  "Tag": "Estimated 401(k)",
  "income": 100000.0,
  "contribution_percentage": 10.0,
  "current_age": 30,
  "age_at_retirement": 60,
  "rate_of_return": 8.0,
  "withdraw_tax_rate": 4.0,
  "estimated_401k": 1841200.032,
  "annual_withdraw_amount": 73648.001
}
```

**GET** `/mortgage_amortization`

- Required parameters : `mortgage_amount`, `mortgage_deposit`,`annual_interest_rate`,`loan_term`
- Sample output

```py
{
    "TAG": "Mortgage monthly payments",
    "mortgage_amount": 250000.0,
    "mortgage_deposit": 25.0,
    "annual_interest_rate": 5.0,
    "loan_term": 25,
    "monthly_payment": 1108.632,
    "Annual_payments": 13303.586
}
```

**GET** `Roth-IRA`

- Required parameters : `principal`,`interest_rate`,`years`,`tax_rate`,`annual_contribution`
- sample output

```py
{
  "Tag": "Roth IRA",
  "Principal":10000.0,
  "Interest Rate": 7.0,
  "Years": 30,
  "Tax Rates": 25.0,
  "Annual Contributions": 5000.0,
  "Roth Ira Balance": 581488,
  "Taxable_saving_balance": 411438,
}
```

=======

**GET** `/enterprise-value`

- Required parameters : `share_price`, `fully_diluted_shares_outstanding`, `total_debt`, `preferred_stock`, `non_controlling_interest`, `cash_and_cash_equivalents`
- sample output

```py
{
    "Tag": "Enterprise Value",
    "Equity Value": 1000.00,
    "Total Debt": 500.00,
    "Preferred Stock": 500.00,
    "Non-Controlling Interest": 1000.00,
    "Cash & Cash Equivalents": 1000.00,
    "Enterprise Value": 2000.00
}
```

**GET** `/salary-calculate`

- Required parameters : `salary_amount`, `hours_worked`, `days_worked` and `payment_frequency`
- Sample output

```py
{
  "Tag": "Calculate Salary",
  "Salary Amount": 400000,
  "Payment frequency": "yearly",
  "Salary": {
    "hourly": 192,
    "daily": 1538,
    "weekly": 7692,
    "bi-weekly": 15385,
    "monthly": 33333,
    "quarterly": 100000,
    "yearly": 400000
  }
}
```

**GET** `/personal_loan`

- Required parameters : `loan_amount`, `interest_rate`, `loan_term_years`, `loan_start_date`
- Sample output

```py
{
    "Tag": "Personal Loan",
    "Loan amount": 20000.0,
    "Monthly payment": 1720.87,
    "Total interest paid": 650.43,
    "Total cost loan": 20650.43,
    "Schedule": "{\"Date\":{\"0\":\"March 2023\",\"1\":\"April 2023\",\"2\":\"May 2023\",\"3\":\"June 2023\",\"4\":\"July 2023\",\"5\":\"August 2023\",\"6\":\"September 2023\",\"7\":\"October 2023\",\"8\":\"November 2023\",\"9\":\"December 2023\",\"10\":\"January 2024\",\"11\":\"February 2024\"},\"Principal\":{\"0\":1621.7,\"1\":1629.74,\"2\":1637.82,\"3\":1645.94,\"4\":1654.11,\"5\":1662.31,\"6\":1670.55,\"7\":1678.83,\"8\":1687.16,\"9\":1695.52,\"10\":1703.93,\"11\":1712.38},\"Interest\":{\"0\":99.17,\"1\":91.13,\"2\":83.04,\"3\":74.92,\"4\":66.76,\"5\":58.56,\"6\":50.32,\"7\":42.04,\"8\":33.71,\"9\":25.35,\"10\":16.94,\"11\":8.49},\"Remaining balance\":{\"0\":18378.3,\"1\":16748.55,\"2\":15110.73,\"3\":13464.79,\"4\":11810.68,\"5\":10148.37,\"6\":8477.82,\"7\":6798.99,\"8\":5111.83,\"9\":3416.31,\"10\":1712.38,\"11\":0.0},\"Principal Total\":{\"0\":1621.7,\"1\":3251.45,\"2\":4889.27,\"3\":6535.21,\"4\":8189.32,\"5\":9851.63,\"6\":11522.18,\"7\":13201.01,\"8\":14888.17,\"9\":16583.69,\"10\":18287.62,\"11\":20000.0},\"Interest Total\":{\"0\":99.17,\"1\":190.29,\"2\":273.34,\"3\":348.26,\"4\":415.02,\"5\":473.59,\"6\":523.9,\"7\":565.94,\"8\":599.65,\"9\":625.0,\"10\":641.94,\"11\":650.43}}"
}
```

**GET* `calculate_lumpsum`
-Required Parameters: `principal`, `interest_rate `, `years`
-sample output

```py
{
    "principal"=10000,
    "interest_rate"=8,
    "years"=5,
     "total_amount": 14693.28,
    "interest_earned": 4693.28
}
```
=======

Add-function-and-endpoint-to-calculate-lump-sum-mutual-fund-investment


**GET** `/FHA_loan`

-Required parameters: `home_price`, `down_payment_percentage`,`loan_term_years`,`interest_rate`,`fha_annual_mip_percentage`
-saample output

```py
{
  "home_price": 200000
  "down_payment_percentage": 10
  "loan_term" (years): 30
  "interest_rate" (%): 3
  "FHA_annual_MIP_percentage" (%): 0.85
  "Down_payment": $20000.00
  "FHA_base_loan_amount": $180000.00
  "FHA_upfront_MIP": $3150.00
  "Monthly_mortgage_payment": $758.89
  "Monthly_MIP": $127.50
  "Total_FHA_loan_amount": $183150.00
  "Total_monthly_payment": $886.39
  "Total_cost_of_loan": $322249.41
}
```

**GET** `/commission_calc`

- Required parameters : Any two of the following as keyword arguements: `amount_paid`, `principle_amount` and `months`
- Sample output

```py
{
  'Tag': 'Commission',
  'Sales Price': 500,
  'Commission Rate': '10%',
  'Commission': 50.0
}
```

```
=======
**GET** `/diluted-earnings-per-share`

- Required parameters : `net_income`, `weighted_avg_shares`, `dilutive_securities`
- Sample output

```py
{
"Tag":"Diluted Earnings Per Share (Diluted EPS)",
"Net Income":1000000.0,
"Weighted Average Shares Outstanding":500000.0,
"Number of Dilutive Securities":100000.0,
"Diluted EPS":"1.6666666666666667"
}
```

=======
**GET** `/refinance`

- Required parameters : `current_loan_amount`, `current_interest_rate`, `current_loan_term_years`, `time_remaining_years`, `new_interest_rate`, `new_loan_term_years`, `cash_out_amount`
- Sample output

```py
{
    "Tag": "Refinance",
    "Current loan amount": 330000.0,
    "Balance left on loan": 170067.93,
    "New loan amount": 169067.93,
    "Current monthly payment": 1826.36,
    "New monthly payment": 1711.73,
    "Monthly savings": 114.63,
    "Current interest paid left": 49095.54,
    "New total interest paid": 36339.74,
    "Total interest saving": 12755.79,
    "Current total cost left": 219163.47,
    "New total cost loan": 205407.68,
    "Total cost saving": 13755.79
}
```

**GET** `/college_cost`

- Required parameters : `book_cost`,`college_tuition`,`Devices`, `travel_expenses`, `hostel_charges`,`mess_fee`,`miscellaneous`
- Sample output

```py
{
            "Tag": "College Cost",
            "Books cost of one year": 5000,
            "College tuition fee per year": 200000,
            "Electronic devices cost":60000,
            "Monthly Travel expenses":4000,
            "Monthly Hostel charges":10000,
            "Monthly mess fee":5000,
            "monthly miscellaneous expenses":3000,
            "Total cost of one year": 529000

}
```
**GET** `/fixed_deposit_maturity`

- Required parameters : `principle_amount`, `years`, `roi`, `compounding` <i>(calculated in monthly ,quaterly ,halfyearly, yearly)</i>
- Sample output

```py
{

            "Tag": "Fixed deposit maturity Amount",
            "Total Value": 138041.98,
            "Principle amount": 100000,
            "Interest anount": 38041.98,
            "Duration in year": 5,
            "Interest Rate": "6.5%",
            "compounding rate": "quaterly"


}
```
**GET** `/recurring_deposit_maturity`

- Required parameters : `principle_amount`, `years`, `roi`, `compounding` <i>(calculated in monthly ,quaterly ,halfyearly, yearly)</i>
- Sample output

```py
{

            "Tag": "Recurring deposit maturity Amount",
            "Total Value": 62494.24,
            "Investment": 5000,
            "Duration in year": 1,
            "Principle amount": 60000,
            "Interest Value": 2494.24,
            "Interest Rate": "7.5%",
            "compounding rate": "monthly"

}
```


**GET** `/calculate_retirement_goals`

- Required parameters : `retirement_age`,`annual_retirement_expenses`,`inflation_rate`,`annual_retirement_income`,`current_age`
- Sample output


```py
{
            "Tag":"Retirement Goals",
            "Retirement age":65000,
            "Annual retirement expenses":50000,
            "inflation rate":0.03,
            "Annual Retirement Income":20000,
            "Current Age":40,
            "Retirement Goals":95010.80947570129
}
```

**GET** `/student_loan`
- Required parameters : 'principal','tenure', 'interest_rate'
- Sample output
```py
{
            "Tag": "Student Loan",
            "Total amount to borrow":300000,
            "total number of years to pay loan":10,
            "interest rate percentage annual":9.2,
            "total monthly cost":3832,
            "Total Amount of loan":459938
}
```


**GET** `/roi_equity_funds`

- Required parameters : `amount_invested`,
    `amount_returned`,
    `tenure`,
- Sample output

```py
{
        
            "Tag": "Calculate return of investments on equity funds",
            "Amount Invested": 1000,
            "Amount Returned": 2000,
            "Duration of investment": 2,
            "Return of Investment": "100%",
            "Annualized Return": "43.88%"

}
```
**GET** `/calculate_gst`

- Required parameters : `price`,
    `gst_rate`,
    
- Sample output

```py
{
        
            "Tag": "Calculate GST and Total Price",
            "Original Price":2180,
            "GST rate":18,
            "Amount of GST": "392.4",
            "Total price after GST":"2572.4"


}
```

**GET** `/asdcr`

- Required parameters :`net_operating_cost`,
  `depreciation`,
  `non_cash_expenses`
  `annual_debt_service`
- Sample output


```py
  {

            "Tag":"Annual Debt Service Coverage Ratio",
            "Annual Debt Ratio":2.0833333333333335,
            "Net Operating Income":100000.0,
            "Depreciation":20000.0,
            "Non Cash Expenses":5000.0,
            "Annual Debt":60000.0
    
  }

```

**GET** `/calculate_vat`
- required parameters : `price`, `vat_rate`
- Sample Request: GET /calculate_vat?price=100&vat_rate=20
- Sample output
```py
{
  "Price (excluding VAT)": 83.33,
  "Price (including VAT)": 100.0,
  "VAT Amount": 16.67

} 
```


**GET** `/loan-affordability`

- Required parameters : `income`,
        `expenses`,
        `loan_term`,
        `interest_rate`,
- Sample Request: `GET`, `http://127.0.0.1:8000/loan-affordability?income=5000&expenses=2000&loan_term=12&interest_rate=5`,    
- Sample output

```py
{
  "income": 5000.0,
  "expenses": 2000.0,
  "loan_term": 12,
  "interest_rate": 5.0,
  "max_loan_amount": 2215.8129091122037
}
```
