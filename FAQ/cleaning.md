#Data Cleaning Tips<br>
Making the model run fast, accurate, and consistent you must spend a lot of time cleaning data. The model's validity is judged by how well it matches live market data.<br>

1.	Cleaning is multi-stage.<br>
	•	Start with obvious issues (like missing or incorrect entries).<br>
	•	Then do finer passes to catch subtle problems until the data is fully usable.<br>
2.	Look beyond just missing values<br>
	•	Missing or nulls are only the first layer of problems.<br>
	•	Data providers might interpolate missing values or record prices in thin markets (low-liquidity, unreliable data).<br>
	•	These require deeper scrutiny.<br>
3.	Clean according to the purpose of the data<br>
	•	Data should be “useful for purpose.” Cleaning should focus on the intended modeling or analysis goal.<br>
4.	Include the broader market context<br>
	•	Don’t only clean or use the data series you’re directly studying. People tend to use data they are interested in.<br>
	•	Include related or background market data - context is essential for realistic modeling.<br>
5.	Iterative evaluation<br>
	•	Cleaning and evaluation should be repeated after each pass to ensure the dataset’s reliability and completeness.<br>
