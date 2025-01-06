# 1.Introduction to Power Bi

power bi desktop -> power bi desktop -> Tile

Power Biservice -> Share file -> Share Dashboard

Power Bi Mobile ->


# 2.How to use power bi from beginner to advanced

install power bi desktop


impoort data from - World Economic Outlook database ->  Gross domestic product, current prices NATIONAL CURRENCY 

url - 

https://www.imf.org/en/Publications/WEO/weo-database/2023/October/weo-report?c=512,914,612,171,614,311,213,911,314,193,122,912,313,419,513,316,913,124,339,638,514,218,963,616,223,516,918,748,618,624,522,622,156,626,628,228,924,233,632,636,634,238,662,960,423,935,128,611,321,243,248,469,253,642,643,939,734,644,819,172,132,646,648,915,134,652,174,328,258,656,654,336,263,268,532,944,176,534,536,429,433,178,436,136,343,158,439,916,664,826,542,967,443,917,544,941,446,666,668,672,946,137,546,674,676,548,556,678,181,867,682,684,273,868,921,948,943,686,688,518,728,836,558,138,196,278,692,694,962,142,449,564,565,283,853,288,293,566,964,182,359,453,968,922,714,862,135,716,456,722,942,718,724,576,936,961,813,726,199,733,184,524,361,362,364,732,366,144,146,463,528,923,738,578,537,742,866,369,744,186,925,869,746,926,466,112,111,298,927,846,299,582,487,474,754,698,&s=NGDP,&sy=2019&ey=2026&ssm=0&scsm=1&scc=0&ssd=1&ssc=0&sic=0&sort=country&ds=.&br=1


go to get data -> web -> paste url ->select table ->  load/transform -> table view

# 3. How to get data from web in power bi

go to home -> use first row as header

select all 'year' columns -> transform -> unpivot column -> change column name to 'Year' & 'Value'


# 4. Power Bi me apna kam save and record kare

 
 go to file -> same as -> savein your local folder 


 remove row (button to remove row)


  to open your report file click - transform data

  to close and go to power bi desktop then - close and apply (left)


  # 5. desktop to Dashboard

  data - https://drive.google.com/file/d/1JmN-C3_6Bugo3rflObKva_rDr2ak-4uM/view


  in place of abc in header column convert to number for year and value


  table view -> column tool -> data category -> select country -> icon will create on right side


  create roport dashboard in report view

  # 6. Power bi Dashboard
  
   chnage 3 setting from check to uncheck


  abc not to detect in power bi - we want to change setting from ourself


  go to files -> options and setting -> options -> data loads 

  remove some checked box to uncheck -> 1,3,5

# 7. Desktop to power bi


4 population files imported


first column as header 
filter - remove n/a from all 4 files - close and apply

# 8. Merge all 4 files and apply query


home - append query (top right) -> append query as new -> all all 4 files and click ok -> rename by double click

# 9. Delete unwanted columns

go to home -> remove column -> remove column

# 10. Prepare power bi dashboard and make visualization

split columns

select column -> transform -> split columns

right click -> create group -> drop all excel file inside it


# 11. Power Bi with new icons

new version that i am using


# 12. Power bi reference option , how to use reference option in power bi

create refernce of original file for further uses - what evver changes u do in main file it will reflect in refernece file but if you did changes in reference file then it wont reflect in main file

click on file -> home -> manage -> reference

and then you can click on right and remove other column -> then righ click on country column and  remove duplicates 

you can not delete main table unless u dont delete reference file



# 13. Edit data in power bi manually || Power Bi Merge query



home -> enter data -> give query name 'Region Code' -> ok

click on 'Region Code' -> right side 'Source' right click on it and then copy data from excel and paste it in the sheet where 'column1' written

now you want to merge 

click on Reference data -> Home -> Merge queries -> merge queries 

select reference data -> region code -> Country -> use fuzzy -> ok 

now click on column right side and select column you want 

# 14. Nested if condition in power bi || How to apply multiple ifs in power bi


to add column  :- Add column -> index column -> 1
duplicate column :- selct column -> add column -> duplicate column
extract number :- selct column -> add column -> extract -> last character
replace value inside column :- home -> replace value(right) -> enter value

Add condition column -> Add column -> conditional column -> ex. age limit <= 4 = child,


# 15. Power Bi remove unwanted files || how to remove unwanted files from power bi visulization

how to multiply by 1000

transform -> standard -> select multiply /subtract


to hide file's in dashboard view

table view -> right side select file (3 dots) -> hide from report view -> now go to reports 
same you can unhide


# 16. Power Bi reduce file size is possible || how to reduce power bi file size || Power bi magic trick


to remove file size -> go to transform data -> file (right click) -> then uncheck enable load


file - Car Produce, Car Sold, Product type




# 17. POWER bI Relationship between tables || power bi relationships tutorial 

to create relation ->  model view 



# 18. Power Bi dax tutorial for beginners || Power Bi functions with examples



excel formula to 
a | 1  ->  a-1 ->          =B2&"-"&C2
b | 2  ->  b-2 ->          
c | 3  ->  c-3 ->          


power bi formula -> column tools -> New columns

column name  = 
Concatenate (A+K) = [Country]&"-"&[Year] 


# 19. Join column without formula by using concatenate

power bi formula -> column tools -> New columns

Excel = CONCATENATE(B2,"-",C2)
      =  CONCATENATE(B2,CONCATENATE("-",C2))

power bi -

Test Formula = CONCATENATE([Country],CONCATENATE("-",[Year]))


# 20. Power Bi dax functions with example | power bi calender table

Table tools -> New tables


formula - Calender Formula = CALENDAR(DATE(2019,1,1), DATE(2020,12,31))

https://learn.microsoft.com/en-us/dax/

now click on right side file and then -> column tool on top -> format -> select format you want

add new coumn and then formula to give month name in different column -
 Column = [One year].[Month]

 Column 2 = [One year].[Quarter]


 # 21. Dax formula if statement 

 Sum, Divide, If formula


table view -> power bi formula -> column tools -> New columns

Sum -> Sales A + B = [Sales A] + [Sales B] 

Divide -> Total % = DIVIDE([Sales A],[Sales A + B],0)   # after that go to format and select percentage

If -> Good-Non Good = if([Total %] > .65,"Good","Not Good")  


# 22. Power Bi related Functions | Dax related functions

Populate Data from different workbook


relationship between two table first with date column (file - Total Revenue, Total Units)

Revenue A = RELATED(Revenue[Item A])


add two columns data 

Revenue A+B = RELATED(Revenue[Item A]) + RELATED(Revenue[Item B])

# 23. Power Bi Dax Vs Measure 

Measure v/s Dax

Dax -> row sum (means it works with rows)
Measure -> column sum (It sum all values of same column)


# 24. Power Bi  Measure  vs calculated columns

file - final Book for measure.xlsx

for measure -> go to table tools -> New Measure 

Revenue A = RELATED(Revenue[Item A]) then go to report view and create report and check sum


# 25. Power Bi measure if statement | if condition in power bi

for measure -> go to table tools -> New Measure 

Total Female sales = CALCULATE(SUM([Total]),FILTER(Sheet1,[Gender] = "Female"))

Total Male sales = CALCULATE(SUM([Total]),FILTER(Sheet1,[Gender] = "Male"))


then go to report view and create report view



# 26. Types of header in Power BI


Report view explore all over header and functionality

# 27. Dax in Power Bi | power bi formulas 

File name - Power BI Dax Total Revenue - 

=LEFT(F2,FIND("@",F2)-1)                   #Michael_Hamilton2594
=RIGHT(F2,LEN(F2)-FIND("@",F2))            # grannar.com

Michael_Hamilton2594@grannar.com

FIRST AND   Last = LEFT([Email address],FIND("@",[Email address])-1)  # =RIGHT(F2,LEN(F2)-FIND("@",F2))  #Michael_Hamilton2594

Last Name = RIGHT([Email address],LEN([Email address]) - FIND("@",[Email address]))  # grannar.com


# 28. Microsoft Power Bi | What is edit interactions


if we have two report view with same x-y axis parameter

Report VIew -> Format -> edit interactions


filter view  


# 29. Power Bi conditional formatting 

report view -> format your visuals -> columns -> color (side click) -> then format (color based formatting)


# 30. Data Dril down in Power Bi | how to drill down in power bi


create herarchiy from right click on column and then drag columns and we can go deeper into graph country wise in all data (drill down)

report view -> Data/drill->



# 31. Designing Dashboard in power bi

dashboarding design


# 32. Power Bi service vs power bi desktop | power Bi service dashboard | Power Bi service gateway
https://www.microsoft.com/en-us/power-platform/products/power-bi


https://app.powerbi.com/groups/me/dashboards/84637748-4582-4e7d-a34b-78246292b357?experience=power-bi



report , dashboard, 
how to share -> go to my workspace -> file-> share


collaborate -> go to workspace -> create workspaces


by installing power bi data gateway we dont have to refresh everytime , we can schedule refresh  


https://powerbi.microsoft.com/en-us/gateway/ - personal mode



# 33. Power Bi dashboard from beginner to advanced

Dashboard - Ajay2 


# 34. Power Bi dashboard frin hindi

Dashboard - Ajay2


# 35. Dispaly percentage and numbers in one power bi graph


File name ->      power bi sample file
report dashboard view -> build view -> line y-axis -> in dropdown -> show values as  -> % of grand total


# 36. Power Bi tips and tricks | create multiple graph in one chart in power bi

first go to new tab of report and -> format your visual -> tooltip (on) -> create pie graph and then come to ur reprot in other page and click on graph and -> format visuals and -> tooltips -> reprot page


# 37. Top 5 Power Bi interview questions

1. how many types of join Kinds we have in power bi

ans - 6 (left outer, right outer , full outer, inner, left anti(rows only in first), right anti(rows only in second ))

file - country code region , region name
home -> merge  query (vlookup)-> merge queries 
checked the last box -'selection matches 258....'

2. What is the difference between Merge and append query

Merge - join two tables (increase columns)
append - if we have 1 , 2 or more tables with same columns names then 
data will get added one by one (increase rows)

Merge Query Multiple all cells and append query divide the cells
Merge query is called Vlookup and can fetch data from different sheet, where in append query append table as per the headers.
Merge query merge all the data and populate only unique values, where in append query only populate unique values
Merge query works only for specific column and append query help us to get all distinct value in one single column.

3. What is the difference between calculated columns and measures?

Calculated columns understand row context.
Measures understand filter context.
Calculated column values are stored in tables.
All of the above


4. What is the difference between Reference and Duplicate sheet? Please write your answer.


right click on file in transform data and we have  Reference and Duplicate options

Reference - whatevver changes we wil do in original sheet it will reflect in Reference sheet
Duplicate - whatevver changes we wil do in original sheet it will  not reflect in Duplicate sheet


5. How to reduce power bi file size ?

go into transform load -> right click and enable the load -> save -> then close tab and go to drive and check size will get reduce