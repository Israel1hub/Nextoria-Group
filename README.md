# Nextoria-Group
# Project Overview.
The Nextoria Group dynamic dashboard delivers a comprehensive overview across three divisions, Technology, Operations, and Commercial, and three regions, AMER, EMEA, and APAC, covering financial performance, customer metrics, people, and operations.
Designed for the executive team, it enables faster and clearer decision-making on hiring, margin pressure, and regional performance. 
The dashboard also eliminates the need for manual tracking across multiple regions and divisions, bringing all critical business data into a single, unified view.

![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/ng1.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG2.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG3.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG4.PNG)
 
# DATA & REQUIREMENT 
There are five relatable tables
1. FactKPI_monthly- Monthlykey,Orgkey, Regionkey,scenario,KPIKey,Value are columns provided.
2. DimRegion - Regionkey,Region, subregion,Country,MarketTier,currency.
3. DimOrg - Orgkey, Division,BusinessUnit, Productline,OrgNodeName,ExecutiveOwner,Isleaf,Orgsort.
4. DimKpi - KPIKey,KPIName,KPICategory, Unit,formatstring,polarity,ExecutiveRelevance,DefaultTargetType.
5. DimDate- Monthkey,Monthstartdate,Year,Quarter,MonthNumber,MonthName,YearMonth,IsBoardseason,FiscalYear,Fiscalquarter.

# PRIMARY OBJECTIVE
Design a clean, executive-focused Power BI report that communicates high-level performance while allowing stakeholders to explore drivers through hierarchy-based drill-down paths.

# THOUGHT PROCESS
KPIkey is used to filter each category based on Revenue,EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization), Headcounts, Net customers adds,   active customers, on-time delivery,system uptime, support ticket, cycle time and Gross margin.

The Scenario column includes Actual, Budget, and Forecast. For growth metrics, the target uses 'Higher' polarity (Actual > Budget). For operation metrics like Cycle Time and Support Tickets, 'Lower' polarity is required.

EBITDA varaince is useed as a dignostic tool to identify underperforming peroductline and pinpoint where profitability is leaking.

The Table chart provides a clear view of customer growth engine by tracking both the "flow" (Net Adds) and the "stock" (Active Customers).

Year and month slicers used to filter the month or year date simultenously, providing the present month and year.

Connected EUR/USD API to Power BI, to automatically convert EMEA currency into USD using real-time exchange rate.

The churn rate was analyzed on a Month-over-Month basis to monitor fluctuations in customer attrition and identify seasonal trends.

HTML code was written and embedded into Power BI conent visual to display the Revenue by region, market Tier distribution and other key KPI.

# ANALYSIS INSIGHT

The overall business is profitable and ahead of plan. EBITDA ( Earnings Before Interest, Taxes, Depreciation, and Amortization) came in $150 million above budget.
Gross margin exceeded the plan by 180 basis points.

Margin pressure, the commercial engine is underperforming While the product delivers strong profit, every sales and marketing function missed its profit target.

This is not six separate problems. It is one structural problem with six visible symptoms; Partnerships, Enterprise Sales, Brand, SMB Sales, Demand Gen,Product Marketing

Commercial is running 1,640 people below its planned headcount. This is an 8.6% miss against a budget of 19,000. Those roles were specifically designed to generate revenue.The direct consequence is a -7.97% profit variance in the Commercial division.

EMEA, half of all Nextoria revenue comes from one region. If EMEA experiences an economic downturn, regulatory disruption, or competitive shift, there is no regional revenue buffer.
 
AMER contributes only 24% of revenue against a typical global expectation of approximately 33%, With 49,521 customers in AMER versus 86,596 in EMEA, the go to market footprint has simply not been built in AMER at sufficient scale. This is likely a direct consequence of the Commercial underhiring problem.

APAC carries 31% of total headcount but generates only 26% of revenue. This means APAC is less efficient than other regions on a revenue per head basis.

March 2026 showed a churn rate of 4.86% nearly double the 2.90% average. This coincides with a sharp spike in support tickets in February and March, and an on-time delivery rate of 91.0% against a 95.0% target.  

System uptime exceeding 100% of target reflects strong engineering reliability and validates the Technology investment.

Over the years, march happens to be the month with the highest number of Net customers adds

# RECOMMENDATION 

The recommendation is a phased hiring plan to close this gap. However; hiring 1,640 people does not fix the profit problem immediately. New hires require onboarding, ramp time, and pipeline building before they generate meaningful revenue in the next Q3 or Q4.

If there are policies imposes on APAC and AMER and not impose on EMEA, let it be lifted as this might have helped EMEA performed well.





