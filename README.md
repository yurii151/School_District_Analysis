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

### Scores by School Spending

Another thing we can look at is how the removal of the grades effects the scores by school spending. The original analysis looked like this:

<img width="841" alt="Screen Shot 2021-11-26 at 3 02 53 PM" src="https://user-images.githubusercontent.com/92888170/143660174-69452a54-75ad-43cf-b815-fde8e865f8bf.png">

and the updated one:

<img width="841" alt="Screen Shot 2021-11-26 at 3 04 37 PM" src="https://user-images.githubusercontent.com/92888170/143660215-deddf930-91e6-48f5-9213-c0101e888d26.png">

For this comparison, we need to look at the row for the spending range of $630-$644 since Thomas High School spends $638 per student.

  - The average math score decreases from 78.52 to 78.50
  - The average reading score increases from 81.62 to 81.64
  - The percent of students passing math decreased from 73.48 to 66.89
  - The percent of students passing reading decreased from 84.39 to 77.48
  - The percent of overall students passing decreased from 62.86 to 56.39

### Scores by School Size

We can also look how this new analysis effects the grades by school size. The original analysis:

<img width="841" alt="Screen Shot 2021-11-26 at 3 11 08 PM" src="https://user-images.githubusercontent.com/92888170/143660434-1a403fd4-16fe-49ca-aa47-36b697d9009a.png">

The new analysis:

<img width="841" alt="Screen Shot 2021-11-26 at 3 12 03 PM" src="https://user-images.githubusercontent.com/92888170/143660484-350d0e0a-f07e-4064-a135-1f11b0a166c6.png">

Thomas High School had an population of 1635 students so we look at how the medium size schools changed
  - The average math score decreases from 83.37 to 83.36
  - The average reading score increases from 83.86 to 83.87
  - The percent of students passing math decreased from 93.60 to 88.33
  - The percent of students passing reading decreased from 96.79 to 91.26
  - The percent of overall students passing decreased from 90.62 to 85.45

### Scores by School Type

The last thing we can analyze is how the dropped grades effected the results of each school type, District or Charter

The original table looked like this:

<img width="718" alt="Screen Shot 2021-11-26 at 3 18 03 PM" src="https://user-images.githubusercontent.com/92888170/143660669-2f9c7685-c102-4f82-a138-a4ac55889067.png">

While the updated one looked a little different:

<img width="718" alt="Screen Shot 2021-11-26 at 3 19 01 PM" src="https://user-images.githubusercontent.com/92888170/143660698-54c90e9c-4f60-4ca5-a8fa-05985f08d9d4.png">

Thomas High School is a charter school so to see the changes we need to look at the charter row:
  - The average math score decreases from 83.473 to 83.465
  - The average reading score increases from 83.896 to 83.902
  - The percent of students passing math decreased from 93.620 to 90.325
  - The percent of students passing reading decreased from 96.586 to 93.131
  - The percent of overall students passing decreased from 90.432 to 87.198

## Summary

After reviewing how the NAN scores effected the school district analysis, we can come to some conclusions. In each case, of each analysis where Thomas High was included, the percentage of students who passed was less than the original analysis. This might be due to the fact that altough the freshman students grades were replaced, we still counted them in the student counts. Another thing that I noticed was that during the new anlysis, the reading grades increased. This means that the freshman at Thomas High were not perfroming well compared to the other grades in reading. I also noticed that after removing the freshman grades, Thomas High School was performing more like a district school even though they had the resources of a charter school. The last thing I noticed was that the medium school average scores didn't change much. THis might suggest that school size, not school buget may be a more important factor in determining how students perform in school. 
