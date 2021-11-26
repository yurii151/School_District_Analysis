# School_District_Analysis

## Summary

This is a continuation of the school district analysis. However, in between the time of this analysis and the last one, it was discovered that there was academic dishonesty being conducted by the freshman at Thomas High School. So in order to correct this, the reading and writing grades of the freshman had to be replaced with Null values, and the analysis had to be conducted again without those scores. 

## Results

### Removing Grades

The first thing that we should look at is how the removal of the freshman grades effects the school district summary. First however, I would like to show how the data was cleaned up to remove the freshman from Thoamas High's. I went through the table using the loc method and logical operators to assign all the grades for reading to NAN. I then did the same thing for the math grades. 

<img width="1010" alt="Screen Shot 2021-11-26 at 2 07 06 PM" src="https://user-images.githubusercontent.com/92888170/143658087-f60204d2-feb8-411f-a6fa-606dc152a110.png">

### District Summary

This lead to a change in the data from the original district summary, which is listed here:

<img width="932" alt="Screen Shot 2021-11-26 at 2 09 10 PM" src="https://user-images.githubusercontent.com/92888170/143658154-197b18fd-05d2-400e-830f-691a4fe483a2.png">

The new district summary looks like this:

<img width="932" alt="Screen Shot 2021-11-26 at 2 10 59 PM" src="https://user-images.githubusercontent.com/92888170/143658219-0ea533a8-eb26-4dde-9410-7281ed2e43a9.png">

Some intersting things to note:

  - The average math score decreased from 79 to 78.9
  - The average reading score didn't change after rounding the figures, it stayed at 81.9
  - The percent of students passing math decreased from 75 to 74.8
  - The percent of students passing reading decreased from 86 to 85.7
  - The percent of students overall passing decreased from 65 to 64.9

### School Summary

Looking at how the new data effects the individual school, here is the original school summary of Thomas High School

<img width="990" alt="Screen Shot 2021-11-26 at 2 21 23 PM" src="https://user-images.githubusercontent.com/92888170/143658677-d104cc8e-01b4-42d9-b24e-5541d3d2698d.png">

The new analysis of the schools gives these results of Thomas High School:

<img width="990" alt="Screen Shot 2021-11-26 at 2 24 17 PM" src="https://user-images.githubusercontent.com/92888170/143658869-4c401aeb-9697-48f0-a5f8-10b50d25edd2.png">

These results are very intersting indeed:

  - The average math score decreased from 83.42 to 83.35
  - The average reading increased from 83.85 to 83.90
  - The percent of students passing math decreased a lot from 93.27 to 66.91
  - The percent of students passing reading decreased a lot from 97.31 to 69.66
  - The percent of students overall passing decreased a lot from 90.95 to 65.08

This big drop is most likley due to the fact that we are missing an entire grades worth of data. 
The removal of the freshman data has a huge effect on Thomas High School's performance, taking it to one of the better performing schools in the district to one of the worse ones. Thomas High School is now the worst performing charter schoool in overall passing %

<img width="990" alt="Screen Shot 2021-11-26 at 2 33 43 PM" src="https://user-images.githubusercontent.com/92888170/143659240-370cff1f-7968-4432-9735-cf3d84d99272.png">

### Math and Reading scores by Grade breakdown

Looking at the grade by grade breakdown changes also leads to some important insights. 

The orignial math grade breakdown by grade per school:

<img width="429" alt="Screen Shot 2021-11-26 at 2 53 24 PM" src="https://user-images.githubusercontent.com/92888170/143659854-6f628aa8-babb-4540-b013-d608b08ea374.png">

The new one:

<img width="429" alt="Screen Shot 2021-11-26 at 2 54 03 PM" src="https://user-images.githubusercontent.com/92888170/143659887-78ec1b67-e6f1-4a2a-93f9-95742219083f.png">


This result is also very interesting:


  - As expected, the grades from Thomas High look alot different. The 9th graders have NaN for their scores, while the averages for the other grades are unchanged.
  - This comparison just confirms that the freshman math grades were properly removed. 
  
We can also look at the reading scores and how they changed in the new breakdown. The original Data table:

<img width="429" alt="Screen Shot 2021-11-26 at 2 56 36 PM" src="https://user-images.githubusercontent.com/92888170/143659983-5be3f660-88d4-4c29-a38e-c2590d20558a.png">

The new one:

<img width="429" alt="Screen Shot 2021-11-26 at 2 57 51 PM" src="https://user-images.githubusercontent.com/92888170/143660025-aa49205a-1f41-4ca4-bde2-30757c7bda47.png">

  - Much like the math grades, the grades from Thomas High reading look alot different. The 9th graders have NaN for their scores, while the averages for the other grades are unchanged.
  - This comparison just confirms that the freshman reading grades were properly removed. 


