# School_District_Analysis

##	Overview of the school district analysis: Explain the purpose of this analysis.
Use Python and the Pandas library to analyze school district data and showcase trends in school performance. Open Jupyter Notebook files from local directories using a development environment, read an external CSV file into a DataFrame. Format a DataFrame column, determine data types of row values in a DataFrame, and retrieve data from specific columns of a DataFrame. Merge, filter, slice, and sort a DataFrame, apply the groupby() function to a DataFrame. Lastly perform mathematical calculations on columns of a DataFrame or Series.
 
## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

- ### How is the district summary affected?

When the Thomas High School 9th grade reading and math scores are removed from the dataset, the total schools and total students numbers were not affected. We still use the same total number of students (39,170) to report overall averages by district. The average math score decreases from 79.0 to 78.9, but the average reading score remains the same (81.9). The percentage of students passing math, reading, and overall percentage is reduced by 1%. This makes sense because there are 461 ninth grade students at Thomas High School, which is roughly 1.1% of the total 39,170 students in the district, it is safe to say that the overall district summary was not largely impacted.


![2022-05-31 (46)](https://user-images.githubusercontent.com/103701561/171259771-23cdfbdd-3e7f-4e60-a76c-98df7bac0c55.png)

  
- ### How is the school summary affected?

The School Summary DataFrame changes Thomas High School itself since we are still using the total number of students in each schools to calculate the percentage of students that pass math, reading, and overall percentage at each school. These percentages will drop for Thomas High School since a quarter of the students will have no score, or a non-passing score, yet they will be included in the total number of students.
	  
- ### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Using the original data set with the corrupted scores puts Thomas High School in the Top 5 schools in the district. Specifically, second in the district with an overall passing percentage of 90.9. However, when the corrupt 9th grade scores are removed from the dataset, Thomas High School drops out of the Top 5 and into the 8th slot with an overall passing percentage of 60.1. This drop is to be expected since the 461 ninth grade students account for 28% of total students at Thomas High School. In this assignment, we were asked to simply replace the corrupt data with NaN’s.

### Top 5 Schools:

![2022-05-31 (37)](https://user-images.githubusercontent.com/103701561/171260994-9ec3b24c-81ff-4e8d-8190-3bdabc14b04b.png)


### Bottom 5 Schools:

![2022-05-31 (38)](https://user-images.githubusercontent.com/103701561/171261090-743ac9b1-c5cb-466c-a265-541890c54a90.png)






### How does replacing the ninth-grade scores affect the following:

- ### Math and Reading scores by grade:

As expected, the math and reading scores by grade for all other schools are not affected when the Thomas High School 9th grade scores are removed. This is due to how the data was grouped into the DataFrame, there is now a hole in the dataset.
  
- ### Scores by school spending:

	Due to how the data was grouped for this DataFrame only the bin that contains Thomas High School is affected. Since Thomas High School’s per student budget is $638, this is the $630-644 bin. Surprisingly, the average math & reading scores stayed the same. Because the total number of students includes the 9th grade students with no scores, the percentage of students passing math, reading, and both overall percentage has dropped in this bin 7 points.
  
- ### Scores by school size:

 Thomas High School has 1,635 students, so it is categorized as a Medium sized school. Here we see a decrease of 6 points in the percentage of students passing math, reading, and both overall percentage.
 
 ![2022-05-31 (47)](https://user-images.githubusercontent.com/103701561/171261805-5108685e-beea-4f29-a944-9ade27088d80.png)
 
 
 
 - ### Scores by school type:

Thomas High School is a Charter School. We see a 4 point drop in the percentage of students passing math, reading, and overall percentage without affecting the District Schools.


![2022-05-31 (48)](https://user-images.githubusercontent.com/103701561/171262155-5620a750-3c51-4621-acfc-f401e1a0ea21.png)







![2022-05-31 (21)](https://user-images.githubusercontent.com/103701561/171213214-5999b36c-8c67-435c-b056-0fdaa6a513bc.png)
![2022-05-31 (22)](https://user-images.githubusercontent.com/103701561/171213234-b4ae238e-c459-4172-8d5d-080918c804a5.png)
![2022-05-31 (23)](https://user-images.githubusercontent.com/103701561/171213255-e98ffea1-9350-4518-84aa-a82b1068f05d.png)
![2022-05-31 (24)](https://user-images.githubusercontent.com/103701561/171213284-81df1323-c5bb-4909-935f-bd310c984c82.png)
![2022-05-31 (25)](https://user-images.githubusercontent.com/103701561/171213306-e176d906-b8c3-4942-b585-696932ae6e43.png)
![2022-05-31 (26)](https://user-images.githubusercontent.com/103701561/171213319-289634ea-7fd2-407c-9e7b-d996e82e9dd0.png)
![2022-05-31 (27)](https://user-images.githubusercontent.com/103701561/171213343-9dfd3a72-17d7-403b-800b-2f458ad785b6.png)
![2022-05-31 (28)](https://user-images.githubusercontent.com/103701561/171213415-6973255e-8774-4507-b823-6e2b9b7e6d8e.png)
![2022-05-31 (29)](https://user-images.githubusercontent.com/103701561/171213441-68b5e865-8353-4cde-8032-03e6cf00328e.png)
![2022-05-31 (30)](https://user-images.githubusercontent.com/103701561/171213478-35f4cb24-9cf5-4525-9f41-06dae66671b1.png)
![2022-05-31 (31)](https://user-images.githubusercontent.com/103701561/171213535-db2ac601-825a-44be-9e66-07e738ab6b31.png)
![2022-05-31 (32)](https://user-images.githubusercontent.com/103701561/171213558-007024da-b3fa-40e9-86b3-b945f2dd8c60.png)
![2022-05-31 (33)](https://user-images.githubusercontent.com/103701561/171213579-1a9884e9-25de-492c-a8ff-cfa579de8462.png)
![2022-05-31 (34)](https://user-images.githubusercontent.com/103701561/171213600-94aba388-5fd2-4472-a0b8-8d486687262c.png)
![2022-05-31 (41)](https://user-images.githubusercontent.com/103701561/171214949-742c10d3-c983-4787-a514-72078e132cbd.png)
![2022-05-31 (42)](https://user-images.githubusercontent.com/103701561/171214995-130aafdf-5024-4d49-8631-be6f63e66313.png)
![2022-05-31 (43)](https://user-images.githubusercontent.com/103701561/171215011-07339073-c6dd-442e-ba85-3aac1c9fde52.png)
