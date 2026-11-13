*1. **Project Overview***



*This project analyses Airbnb listings and review data across ten international cities to understand market performance, pricing patterns, property distribution, host performance, and customer review activity.*



*The project uses PostgreSQL for data preparation, validation, and SQL analysis, and Microsoft Power BI for interactive dashboard development and visualization.*



*2. **Project Objectives***



*The objectives are to:*



*- Examine Airbnb listing distribution across cities.*

*- Analyze room types and property categories.*

*- Investigate listing prices within individual cities.*

*- Identify neighborhoods with high listing concentrations.*

*- Examine host response and acceptance rates.*

*- Analyze review activity and listing ratings.*

*- Identify characteristics associated with higher-priced listings.*

*- Present findings and recommendations through an interactive dashboard.*



*3. **Tools and Technologies***



*- PostgreSQL: Data storage, cleaning, validation, and analysis.*

*- pgAdmin 4: Database management and SQL execution.*

*- Microsoft Power BI Desktop: Data modelling, visualization, and dashboard development.*

*- Microsoft Word: Project documentation.*

*- Microsoft Excel: KPI definition sheet.*



*4. **Dataset Description***



*The project uses two datasets:*



***Listings dataset***

*- Original records: 279,712*

*- Contains listing details, location, property type, room type, pricing, host information, and review scores.*



***Reviews dataset***

*- Original records: 5,373,143*

*- Contains review IDs, listing IDs, review dates, and reviewer IDs.*



*5. **Data Preparation and Modelling***



*The datasets were imported into PostgreSQL and prepared for analysis.*



*The following tables were created:*



*- `airbnb.listings\_raw`*

*- `airbnb.reviews\_raw`*

*- `airbnb.listings\_clean`*

*- `airbnb.reviews\_clean`*



*The cleaned tables contain appropriately typed fields for analysis.*



*A one-to-many relationship was established between Listings and Reviews using `listing\_id`.*



*All review listing IDs matched existing listing IDs in the Listings dataset.*



***6. Dashboard Structure***



*The Power BI dashboard contains four pages:*



*1. Airbnb Market Overview: Listing distribution, total listings, total reviews, room types, and property types.*

*2. Pricing and Property Analysis: Average and median prices, accommodation capacity, and property characteristics.*

*3. Host Performance Analysis: Host response rates, acceptance rates, superhost distribution, and host listing counts.*

*4. Review Activity and Listing Scores: Review trends, most-reviewed listings, and listing ratings.*



*Interactive filters were included to support exploration of the dashboard.*



*7. **Key Findings***



*- Paris has the highest number of listings, with 64,690.*

*- Entire-place listings account for approximately 65.07% of all listings.*

*- Entire apartments represent approximately 49.69% of all property types.*

*- Review activity reached its highest level in 2019, with 1,633,546 reviews.*

*- Cape Town recorded the highest average host response rate at 90.76%.*

*- Bangkok recorded the highest average host acceptance rate at 90.52%.*

*- Entire-place listings have a higher average accommodation capacity than private rooms.*



*8. **Validation***



*Three key dashboard calculations were independently checked against PostgreSQL results:*



*- Total listings: 279,712.*

*- Total reviews: 5,373,143.*

*- Reviews in 2019: 1,633,546.*



*All three calculations matched.*



*Dashboard filter interactions and the Listings-to-Reviews relationship were also tested.*



*9. **Important Limitations***



*- The dataset does not provide a currency column. Prices should therefore be interpreted within individual cities rather than compared directly across cities.*

*- Review data ends on 1 March 2021, making 2021 a partial year.*

*- Some host information and review scores contain missing values.*

*- Some listing names and neighbourhood labels contain character-encoding inconsistencies.*



*10. **Project Folder Structure***



*The project files are organised as follows:*



*Airbnb\_Market\_Analysis/*



&#x09;*SQL\_Queries*

&#x09;	*01\_data\_exploration.sql*

&#x09;	*02\_data\_cleaning.sql*

&#x09;	*03\_data\_validation.sql*

&#x09;	*04\_business\_analysis.sql*

&#x09;	*05\_summary\_views.sql*



&#x09;*Dashboard*

&#x09;	*Airbnb\_Market\_Performance\_Dashboard.pbix*



&#x09;*Screenshots*

&#x09;	*01\_Airbnb\_Market\_Overview.png*

&#x09;	*02\_Pricing\_and\_Property\_Analysis.png*

&#x09;	*03\_Host\_Performance\_Analysis.png*

&#x09;	*04\_Review\_Activity\_and\_Listing\_Scores.png*



&#x09;*Documentation*

&#x20;   		*Airbnb\_Data\_Quality\_Assessment.docx*

&#x20;   		*Airbnb\_KPI\_Definition\_Sheet.xlsx*

&#x20;   		*Airbnb\_Validation\_Evidence.docx*

&#x20;   		*Airbnb\_Executive\_Summary.docx*





*11. **Conclusion***



*This project demonstrates the use of SQL and Power BI to prepare, analyse, validate, and visualise Airbnb market data. The dashboard provides insights into listing distribution, pricing patterns, host performance, and customer review activity across the selected cities.*

