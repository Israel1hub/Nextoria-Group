# Nextoria-Group
## Project Overview.
The Nextoria Group dynamic dashboard delivers a comprehensive overview across three divisions, Technology, Operations, and Commercial, and three regions, AMER, EMEA, and APAC, covering financial performance, customer metrics, people, and operations.
Designed for the executive team, it enables faster and clearer decision-making on hiring, margin pressure, and regional performance. 
The dashboard also eliminates the need for manual tracking across multiple regions and divisions, bringing all critical business data into a single, unified view.
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/ng1.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG2.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG3.PNG)
![image alt](https://github.com/Israel1hub/Nextoria-Group/blob/f5961f5b4ef314fe14d1b509789c79aefa4c62ab/NG4.PNG)
 
# DATA & REQUIREMENT 
There are five relatable tables
**.** FactKPI_monthly- Monthlykey,Orgkey, Regionkey,scenario,KPIKey,Value are columns provided.
**.** DimRegion - Regionkey,Region, subregion,Country,MarketTier,currency.
**.** DimOrg - Orgkey, Division,BusinessUnit, Productline,OrgNodeName,ExecutiveOwner,Isleaf,Orgsort.
**.** DimKpi - KPIKey,KPIName,KPICategory, Unit,formatstring,polarity,ExecutiveRelevance,DefaultTargetType.
**.**DimDate- Monthkey,Monthstartdate,Year,Quarter,MonthNumber,MonthName,YearMonth,IsBoardseason,FiscalYear,Fiscalquarter.

# PRIMARY OBJECTIVE
Design a clean, executive-focused Power BI report that communicates high-level performance while allowing stakeholders to explore drivers through hierarchy-based drill-down paths.

# THOUGHT PROCESS
KPIkey is used to filter each category based on Revenue,EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization),Headcounts,Net customers adds, active customers, on-time delivery,system uptime,support ticket,cycle time and Gross margin.

Scenario consists of Actual, Budget and forcast. The default target type focuses on budget which the polarity needs to be higher.

