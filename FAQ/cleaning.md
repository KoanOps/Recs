# Data Cleaning Tips<br>
Data cleaning is not the sexiest job and often seen as "dirty work". But it is absolutely essential, maybe ~90% of the actual manhours. Making your model run fast, accurate, and consistent - you must spend a lot of time cleaning data. Your model's validity is judged by how well it matches live market data.<br>

1.	Cleaning is multi-stage.<br>
	•	Start with obvious issues i.e. missing or incorrect entries<br>
	•	Then, do finer passes to catch subtle problems until the data is fully usable<br>
2.	Look beyond just missing values<br>
	•	Missing or nulls are only the first layer of problems<br>
	•	Data providers might interpolate missing values or record prices in thin markets i.e. low-liquidity, unreliable data<br>
	•	This requires deeper scrutiny<br>
3.	Clean according to the purpose of the data<br>
	•	Cleaning should focus on the intended modeling or analysis goal<br>
4.	Include the broader market context<br>
	•	Don’t only clean or use the data series you’re directly studying, people tend to use data they are interested in<br>
	•	Include related or background market data, context is essential for realistic modeling<br>
5.	Iterative evaluation<br>
	•	Cleaning and evaluation should be repeated after each pass to ensure the dataset’s reliability and completeness<br>

# Caveat<br>
Please note this is meant to be introductory. Expertise is from learned experience - know by knowing what you're doing, knowing where to look, how to ascribe soundness to the data, and so on. Look at the data, understand the market/business. Dive into how and where the data was created, what all the codes mean, puzzle match, identify patterns, fix those patterns, and bring that dataset into a more uniform set. <br> 

As an example, 5000 lines of messy, inconsistent, unvalidated mortgage data with complex inter-dependencies may take 50-500 manhours, depending on the complexity. <br> 

A word of caution - you may be tempted to do an "automated" solution. This will depend on the dataset and the approach. Automation of data cleanup in this example can far exceed the manhours of **just working manually**. Automation as a substitution for due diligence tends to not go well. [1] <br>

[1] https://xkcd.com/1319/
