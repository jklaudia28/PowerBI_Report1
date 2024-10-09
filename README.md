# PowerBI_Report1
Power BI report is based on my own data from xlsx files.
It contains three sheets:
1) Sales overview
2) Product Analysis
3) Region Analysis

Report contains measures (with conditional formatting), filteres & parameters written both - in DAX and Tabular Editor.
![image](https://github.com/user-attachments/assets/b97f0464-09fd-4595-b7b3-324375804b4b)

Time intelligence calculation item example:
VAR WCZORAJ = today() - 1 
RETURN
CALCULATE (
    SELECTEDMEASURE (),
    FILTER (  'Calendar' , 'Calendar'[DATE] = WCZORAJ )
)

![image](https://github.com/user-attachments/assets/4a61c0e7-f6be-4478-b1eb-3452e7fef00a)

![image](https://github.com/user-attachments/assets/8b5b5a47-bb9c-4bdd-bb69-324c0c1308c2)
