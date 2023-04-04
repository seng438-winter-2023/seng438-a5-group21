**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#21:      |     |
| -------------- | --- |
| Student Names: | Tony Tan |
|                | Evan Wong |
|                | Johnny Yuen |
|                | Bryant Zhang |

# Introduction

In this lab, we aim to gain hands-on experience on assessing the reliability of software systems through collecting data of failure during testing. This is done through reliability growth assessment such as CASRE or SRTAT and reliability assessment using Reliability Demonstration Chart. This will allow an understanding of the usefulness of reliability growth testing, ability to measure failure rate through analysis of MTTF and reliability of SUT, and become more experienced with reliability growth testing tools.

# Assessment Using Reliability Growth Testing 
**Result of model comparison (selecting top two models)**    
![image](https://user-images.githubusercontent.com/101444825/229654587-84139f13-4fdf-44ab-9e31-2573b69c58be.png)   
Performing Trend Analysis Using Geometric model   


![image](https://user-images.githubusercontent.com/101444825/229654624-0c6827fe-8dfd-47ad-add6-ee86b4bac4e3.png)   
Performing Trend Analysis Using Littlewood and Varral’s Bayesian Reliability

The data we tested is Failure Report 2. The top two models were Geometric and Littlewood and Varral’s Bayesian Reliability. This is because they were the only models that worked on our machine and for our data set.

**Result of range analysis (an explanation of which part of data is good for proceeding with the analysis)**    
**Plots for failure rate and reliability of the SUT for the test data provided**   

![image](https://user-images.githubusercontent.com/101444825/229654683-a46850ac-de6c-4611-bbf3-255d981071d5.png)

![image](https://user-images.githubusercontent.com/101444825/229654695-75bd598d-f44e-4524-a17d-2d7c76604af7.png)

**A discussion on decision making given a target failure rate**   
As shown in the failure intensity graph, the failure rate increases at around 3 failures. It then generally decreases as time goes on and the number of failures increases. 
As shown in the mean time between failures vs failure number graph, an increasing series of arithmetic mean indicates reliability growth. This shows that as time goes on, the SUT becomes more reliable.

# A discussion on the advantages and disadvantages of reliability growth analysis

 **Advantages of reliability growth analysis**
* Provides information and data to improve a system’s reliability
* Determines the reliability of a product
* Can compare the reliability of multiple products

**Disadvantages of reliability growth analysis**
* Requires a large amount of data to provide accurate analysis
* Requires a large amount of time and effort to understand
* Can provide inaccurate information if not analysis not completed properly
* Requires additional tests to determine useful ranges of data


# Assessment Using Reliability Demonstration Chart 
For the assessment using the reliability demonstration chart, we used the provided excel spreadsheet. We substituted the sample data for the real failure data provided in the word documents. The plots for minimum MTTF, half and twice are shown down below for our data. Some data was combined and cut to make sure the plot worked well and to show a clearer picture of the data analyzed. The excel spreadsheet also had to be modified in some areas in order to successfully display data.

3 plots for MTTFmin, twice and half of it for your test data
Minimum MTTF: 100/70000 = 0.00142857142

![image](https://user-images.githubusercontent.com/101444825/229654980-374c5d9c-ab98-4dd5-919f-4856cd5a623f.png)

Double MTTF:  100/140000 = 0.00071428571

![image](https://user-images.githubusercontent.com/101444825/229654998-5f56335e-e117-45aa-a91d-f1fa557989ed.png)

Half MTTF: 100/35000 = 0.00285714285

![image](https://user-images.githubusercontent.com/101444825/229655031-c42c03a7-a1c7-4343-873a-e9865ad8ccaa.png)

**Explain your evaluation and justification of how you decide the MTTFmin**
How we decided the MTTFmin of our graph was first inputting our failure data into the reliability demonstration chart tables within the excel sheet. Then adjusting the time per cycle over and over narrowing down until an acceptable result was found continuously looking between the failure data and demo chart. We opted for a result where the last data point would eventually reach outside of the continue, and into the accept. This means our software has met acceptable standards.


**Discussion on the advantages and disadvantages of RDC**   
The advantages of using RDC is that it provides a visual and graphical way to present the data, which can help more clearly represent the data to people who aren’t acquainted with more advanced software and techniques. Also it is very simple to use as it is all stored in a single excel sheet, as well as fast as all you need to do is input failure data. Finally it’s extremely easy to interpret with many basic settings to make sure the reliability information is conveyed appropriately. 
     
The disadvantages of using RDC is that without enough data it becomes virtually useless, as large sample sizes are needed to fully visualize and interpret the results. Also while being simple, easy and fast it will limit the accuracy of the results as it cannot show more in-depth specifics. Finally some of the settings within the RDC are assumptions, so human error can become a problem when inputting data.

**Comparison of the results with the Part 1**
The software SUT being tested seems to be reliable, as in both methods of assessment, reliability growth testing, and reliability demonstration chart gave similar results when analyzing the failure data. When performing assessment using RDC, the majority outcome is close to the acceptance range, meaning the system is performing adequately, but there is room for improvement. When performing assessment using RGT, with failure in respect to time gave a clear perspective on failure intensity. Both assessments provide a clear understanding in both visual and conceptual reliability of a system.


# Comparison of Results
The software SUT being tested seems to be reliable, as in both methods of assessment, reliability growth testing, and reliability demonstration chart gave similar results when analyzing the failure data. When performing assessment using RDC, the majority outcome is close to the acceptance range, meaning the system is performing adequately, but there is room for improvement. When performing assessment using RGT, with failure in respect to time gave a clear perspective on failure intensity. Both assessments provide a clear understanding in both visual and conceptual reliability of a system.


# Discussion on Similarity and Differences of the Two Techniques
Both assessment of reliability growth testing and reliability demonstration chart aim to calculate and give a clear picture and understanding of software reliability through data inputs. However the data inputs are different, and have to be modified. The two assessments differ in that the data to assess reliability is different. RDT data must be prepared and formatted, resulting in outputs with detailed information which can be displayed differently. RDC uses MTTF and risks for assessment, using data entered into excel a graph is generated, this limits the output detail and information. Providing limited options for displaying the data compared to RDT. 

# How the team work/effort was divided and managed
The Teams management of work and effort was divided and through firstly splitting into teams, and allocated tasks evenly and fairly between the two groups with a timeline of tasks. Using the method of peer programming the team aimed to increase efficiency and decrease mistakes when performing reliability assessments. After everything was complete, we combined the work together and tested and ensured as a group that everything was working correctly, sharing our experiences together.


# Difficulties encountered, challenges overcome, and lessons learned
Major difficulty encountered during this lab is the lack of instruction or clear instruction when setting up this lab. Many parts seem to be missing, lack of explanation or examples were not provided. This led to the team having to make many assumptions, trial and errors. A need to become more familiar with tools provided from the lab was needed along with making assumptions for this lab.


# Comments/feedback on the lab itself
This lab helped gain good understanding and experience through being hands-on with reliability growth testing tools. It gave good insight into the two assessment methods (growth testing and demonstration chart), and their similarities and differences. This gives users options for when it comes to assessments of software reliability. This lab also gave the team a good opportunity for teamwork. However, this lab was difficult to set up since instructions were not very clear, detailed step by step guide and examples would have been beneficial and time efficient. The tools used were hard to navigate.

