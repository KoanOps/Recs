Data Cleaning Tips<br>
Making the model run fast, accurate, and consistent you must spend a lot of time cleaning data. The model's validity is judged by how well it matches live market data.<br>

1.	Cleaning is multi-stage.
	•	Start with obvious issues (like missing or incorrect entries).
	•	Then do finer passes to catch subtle problems until the data is fully usable.
2.	Look beyond just missing values
	•	Missing or nulls are only the first layer of problems.
	•	Data providers might interpolate missing values or record prices in thin markets (low-liquidity, unreliable data).
	•	These require deeper scrutiny.
3.	Clean according to the purpose of the data
	•	Data should be “useful for purpose.” Cleaning should focus on the intended modeling or analysis goal.
4.	Include the broader market context
	•	Don’t only clean or use the data series you’re directly studying. People tend to use data they are interested in.
	•	Include related or background market data - context is essential for realistic modeling.
5.	Iterative evaluation
	•	Cleaning and evaluation should be repeated after each pass to ensure the dataset’s reliability and completeness.
