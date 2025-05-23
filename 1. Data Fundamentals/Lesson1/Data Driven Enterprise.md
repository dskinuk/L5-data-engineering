# Notes for Data Driven Enterprise   

The key sub modules for this lesson are as follows:
1. Fundamentals of data driven enterprise
  - Think of any metrics that could be tracked to provide valuable data driven insights
    - An example for this could be a Value dashboard for all the products the team builds. 
    - Metrics could be User personas who use the product
    - Use cases for using the product
    - FTE saving, 
    - decision points it helps to serve
2. Building a datadriven culture
  - Provide strategies for fostering a data driven culture
    - Build strong relationships with your stakeholders - Building customer journeys with them and keeping them involved in the process
    - Transparency in algorithms - Develop User manuals or videos that explain the logic in business terms. 
    - Celebrating and embracing small wins - This helps improve cohesion and provides tangible evidence to persuade initially sceptical stakeholders
    - Raising Data Literacy - Providing foundational training in statistics and analysis. 
      However this linked to the point above as these training intiatives will only help if there is a productive buy-in from stakeholders
3. Value of data and Manage different data types and sources

A. Big data is like an ocean while small data is a Lake which crystal clear
  - Transitioning to big data - As orgs grow the data grows as well and there may be a need to transition from small data to BIG DATA due to
    - Overwhelming data - Systems have grown exponentially and thus are proving inadequate
    - Performance bottlenecks - Expanded volumes impact performance. Also the processing techniques required may also impact performance
    - Missed Opportinities - Inavailability of the right data for predictive insights and trends analysis which aid strategic planning
  - Characterisctics of Data - Five `V's`
    - Volume - quantity of data - Big data(typically TB or PB) - Small data - (typically MB or GB)
    - Variety - data types and sources and whether it is unstructured/semi-structured or structured.
      - Big data - multiple sources like social media sensor networks leading to different formats and structutes.
        In the example of the Value dashboard, data from different product labs who use different tools to build and store data
      - Small data is often well structured and has a uniform source and system.
    - Velocity - speed of data creation and processing - 
        Big data may require real time response as the speed of data creation and processing is high
        Small data is generated at slower spped and thus may require batch processing or periodic processing.
    - Veracity - accuracy and reliability of data
        Big data - Can becoming noisy and inaccurate due to incomplete or erroneous data and thus ensuring their quality and integrity is crucial
        Small data - higher data quality as tighter contraints and easier to validate and clean
    - Value -  insights and benefits that can be derived
        Big data - higher potential to provide valuable insights, by trend analysis, predictive modelling for strategic decision making.
        Small data - delivers immediate value for day to day decision making
data sizes - Bytes(B), Kilobytes(KB), Megabytes(MB), Gigabytes(GB), terabytes(TB), Petabytes(PB),exabytes(EB), Zettabytes(ZB), Yottabytes(YB)

B. Data types

  - Quantitative - anything that can be described as a number
    - discrete - can count
    - continuous - can measure
  - Qualitative - anything that cannot be described as a number
    - Binomial - Boolean values e.g. yes/no, True/false
    - Nominal - Named data e.g. UK/US/France (like list options?)
    - Ordinal - has an order e.g. Small medium Large/Poor Average Good/ Low medium high highest
4. Significance of standards,best practices, regulations
Data formats  - JSON - lightweight human readbale for transmitting data between servers and web apps
              - CSV - Comma separated version - storing tabular data to process and analyse
              - XML - Markup Language - structuring and exchanging data between systems
API - Application Program Interface - enable interconenction of digital systems and data excahnge e.g. integrating third party interface with internal application
        - Restful API design principles - client server architecture to design networked apps and resource based URLs
        - Open API - ???
5. 3 fundamental principles of data Stewardship are:
    - Data Quality
    - Data Governance
    - Data Ethics
6. Engineering best practices for data systems include scalability, reliability, security, performance optimisation, and documentation

7. The data management lifecycle involves 
  - collecting data from sources, 
  - cleaning/transforming data, 
  - integrating datasets, and 
  - visualising insights using tools like SQL, Power BI, and Tableau

Tasks - arrange a meeting with Senior Data engineer in the team to understand the different types and data sources
Outline approach of learning standards, best practices and regulations which inform the use of data systems in the org
