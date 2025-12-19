This project is related to Dairy sciences. It involves modelling events based on certain properties of cows. 
The dataset needed to work with was prepared in the following way.

1. afi_base_data was used as the reference data.
2. For each cow, date ranges comprising of 30 days before the minimum date (start date) and 30 days after the maximum date (end date) was created.
3. For thos date ranges, the fields bacteria, type and gram were populated with the same values corresponding to the start date and end date values for dates 30 days before and 30 days after respectively.
4. Runimation index and water intake data was fetched for the relevant cows. Only the values corresponding to timestamp 00:00 for each cow was considered.
5. For yield and conductivity, date was filled using afi_after_data and posthmus_data.
6. Using the events data, for each cow and date pair, the events were matched and grouped as a list of events (there were instances where multiple events were mapped to the same cow and date pair)

