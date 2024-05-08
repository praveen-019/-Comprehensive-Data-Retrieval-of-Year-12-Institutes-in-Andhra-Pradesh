# -Comprehensive-Data-Retrieval-of-Year-12-Institutes-in-Andhra-Pradesh

# Objective:
To collect information like (Name of the Institute, Location/ Address, Contact Number, Email ID) on Junior Colleges/High Schools/Private Institutes offering Year 12 education in Andhra Pradesh.

# Methodology:

# Web Scraping:
Utilized Python's requests library to send GET requests to the official website of the Board of Intermediate Education, Andhra Pradesh (BIEAP).
Employed BeautifulSoup for HTML parsing to extract relevant information from the web pages.

# Data Retrieval Functions:
## Function_1: retrieveInfoFromCollege
Developed a function to retrieve information (college name, location, phone number) from the official website of the Board of Intermediate Education, Andhra Pradesh (BIEAP) for a given college name.
Extracted relevant information and formatted it before adding it to the CSV file.
##Function_2: retrieveCollegeFromMandal
Created a function to extract information on colleges present in each mandal, including colleges in different villages within the mandal.
Stored mandal information in a list and called the retrieveInfoFromCollege function for each college name to collect detailed information.
Utilized a hierarchical approach, starting from mandals, to gather comprehensive data.
##Function_3: retrieveMandalFromDistrict
Developed a function to extract all mandals present in a particular district.
Stored mandal information in a list and called the retrieveCollegeFromMandal function for each mandal to collect college data.

#Execution:
Initiated data retrieval from the district level, progressing downwards to mandals and then to individual colleges.
Implemented error handling to manage cases where tables or required data were not found on web pages.

#Results:
Successfully retrieved comprehensive data on Year 12 educational institutes in Andhra Pradesh.
Organized data into a CSV file, including college name, location/address, contact number, and email ID.

#Conclusion:
This project demonstrated the effective use of web scraping techniques to gather detailed information on Year 12 educational institutes in Andhra Pradesh. By systematically navigating through districts, mandals, and colleges, the project achieved comprehensive coverage. The collected data serves as a valuable resource for educational research, analysis, and decision-making processes.
