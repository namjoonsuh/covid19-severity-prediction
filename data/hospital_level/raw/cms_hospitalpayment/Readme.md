- Data source: In the webpage https://www.cms.gov/OpenPayments/About/Resources with the download link https://www.cms.gov/OpenPayments/Downloads/2020-Reporting-Cycle-Teaching-Hospital-List-PDF-.pdf
- Last downloaded: 04-01-2020
- Description: This data has TIN, business addresses and hospital cost addresses about each hospital.
- Known data quality issues: 
    - There are two addresses for each hospital and it is not clear which one to use.
- Selected Columns:
    - CCN: int, CMS control number, CMS is the Center for Medicare-Medicaid Services (CMS)
    - TIN: int, Taxpayer identification number
    - Hospital Name: str, Name of a hospital
    - PECOS Legal Business Name: str, a hospital's registered name at IRS
    - Street Address: str, Address as appears on hospital cost report, This address should be understood as the address of the office of the hospital. For a chained hospital or a hospital whose office is different from the actual location of the hospital, this address might not match with the hospital's business address.
    - PO Box: int, Address as appears on hospital cost report
    - City: str, Address as appears on hospital cost report
    - State: str, Address as appears on hospital cost report
    - Zip code: int, Address as appears on hospital cost report, since the zip code is as an int, preceding zeros are removed. 
    - Street Address 1/2, City.1, State.1, Zip Code.1: str,  NPPES Business Address where NPPES stands for National Plan and Provider Enumeration System. It is a system developed by CMS.
