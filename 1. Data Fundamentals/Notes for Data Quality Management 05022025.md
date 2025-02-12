# Data Quality Management

## Introduction to Data Quality

Data Quality is the foundation of a strong and resilient data driven enterprise
It encompasses some key dimensiosn or metrics and they are abbreviated as :
**CIAT**

-- **C** - **Consistency** - How well does the data conform to standards(Uniformity)
  
-- **I** - **Integrity** - How you can ensure that remains accurate and consistent throughout the lifecycle (Completeness)

-- **A** - **Accuracy** - How well does the data represent the real world(correctness, validity)

-- **T** - **Timeliness** - How uptodate is the data(recency) 

Over a period of time another high level metric can be used ***RELIABILITY***
Which measures how dependable and trustworthy the data is?

## Data and Meta Data Standards   

Like a map enables people travelling by different modes in different geographic locations to travel and reach their destinations, the standards ensure that data across multiple systems stays aligned and can interact between varied systems and toolsets.

**Open standards** - They are used by multiple engineers across various use cases and they can contribute to them as well to ensure that:

  - ***Compatibility*** - Different systems and tools can talk to each other
  
  - ***Flexibility*** - Are free to use varied products and toolsets from different companies
  
  - ***Innovation*** - Encourages new ideas by allowing everyone to contribute to these standards
  
  - ***Cost effective*** - Often free to use and thus save costs to companies

Thus fosters a collaborative environment for engineeers to innovate cost effective tools for data management that can be 
seamlessly integrated and evolved. 

### Some examples of Open standards are:

- Industry specific - (HL7 for health care industry)
- Cross Industry - (HTTPS/TCPIP)
- Open data standards (ODATA, OPEN API)

Some standards used in the bank:

- ISO20022
- FIX - the language of the global financial markets used extensively by buy and sell-side firms, trading platforms and even regulators to communicate 

**Fair Standard**

Fair data are data that meet:
- ***Findability*** - Data can be easily found by authorised users. Cataloging data and assigning unique identifiers
- ***Accessibilty*** - Access management to ensure the right people have the right access to the data at all times
- ***Interoperability*** - Ensure data can be integrated across systems. Ensure uniform formats and adoption of common standards across the board.
- ***Reusability*** - Ensure the metadata for the data is accurate and available across systems so that the data can be re-used without having to re-collect and create inconsistencies.

Open Meta Data - Is a standard toolkit that helps to develop Metadata maps
These maps provide crucial support to data engineers about the meaning, context, background and any contraints for the data

Some exmaples of existing data standards are:
- Open Banking standards - define technical specifications and APIs for sharing banking information between banks and third parties.
- NHS Digital Interoperability Toolkit - provides guidance and standards for interoperability between different healthcare systems
- UK Data Service - repository of socio econic data to share best practices across teams and data management frameworks.

- **DCMI** Dubline Core MetaData Intiative
  Used mostly to develop deta data for digital data assets like documents, images, videos, web pages etc.

  Most popular use caes of Dubline core:
  - Museums and archives
  - Digital Publishing
  - British Library
  - Goverment data - gov.uk portal
      -- HMRC account sign in
      -- Universal credit account
      -- Self assessment tax return

Challenges of Unstandardised data
- data Silos - without standardisation data often gets silo'd in different departments
- inconsistent data - Silo'd data is at risk of becoming in consistent
- Integration issues - This further leads to issues in integrating data acrodd different systems
Standards help overcome these challenges by:
- ***Facilitating Data Sharing*** - provide common frameworks that allow sharing across multiple systems and organisations 
- ***Promoting Collaboration*** - standard formats and protocols allow seamless collaboration ensuring all parties interpret data consistently  
- ***Enhancing Interoprability*** - definition of common data models and protocols allows diverse systems to communicate effectively
- 

## Data Formats
  - XML - Extensible Markup Language - Markup language developed to structure and exchange data between systems.
  - CSV - Comma Seperated Value - Storing and exchanging tabular data across systems for data analysis
  - JSON - Java Script Object Notation - lightweight human readable for transmitting data between servers and webpages

The above formats pose different data quality issues which need to be known to decide which format is best in a particular situation/use case.

Structured Data                  Unstructured data
- Relational database             - Not in Relational database
- Predefined structure            - No predefined structure
- Highly organised                - Stored in Data warehouses/Lakes
- Easy to scale/access/store      - Significant chanllenges to store/scale
- e.g. Spreadsheet                - Social media data, audio or video data

### Choosing a Data Format 

To decide what data format best suits the purpose, may require assessment on the following:

- **Structured/Unstructured/semi-structured Data** - How is the data
- **Use Cases** -  What is the purpose of the data
- **Tooling and ecosystem** - What Tools are available for a format
- **Performance** - What are expected performance levels
- **Interoperability** - How is the data expected to be available across varied systems
- **Security** -  Expected levels of security and access controls
    
- Navigating Quality Issues in XML formats
    - Parsing issues due to complex and nested structures and mismatched tagging -
      - Mitigation - Using effective parsers and reviews and testing
    - Character encoding due to unrecogisable special characters
      - Mitigation - Ensuring special characters are used with the character equivalents
    - Schema Validation Issues due to inability to directly call out validation rules
      - Defining and testing scheme validation
     
- Navigating Quality Issues in CSV formats
    - Lack of standardised Schema leading to inconsistencies in data representation across different files
      Header misalignment can lead to to errors i data mapping
        - ensure all CSV have consistent headers and alignment
    - Does not support explicit data types
      - provide metadata to support the CSV file to help identify the type of data
    - Fragilty - susceptible to errors due to inconsistent delimiters, line terminators etc.
      - Mitigation - standardise use of delimiters, encapsulators and line terminators
      
***API - Application Programming Interface - Is a set of tools, protocols that specify how software components communicate/interact with each other. A sort of messenger for different apps to talk to each other. 
e.g. When we use a mobile app to book a taxi, our app communicates with the taxi company's server through an API to request and recive info avout available drivers, faresmm estimated arrival times etc.
    
- Navigating Quality Issues in JSON formats
    - No built in mechanism to define schema - can lead to data validation issues
        - Mitigation - Key Value pair integrity - commonly used to organise and represent data.
        - COnsistent key naming is eesential to ensure that integrity is maintained
          Engineers must establish naming conventions and validation rules to maintain key vaue pair integrity
    - Limited data Types - may not support all types of data
    - Complex Nesting may complicate parsing leading to performance issues
        - Mitigation - Carefully design JSON strcutures to balance complexity with efficiency
    - data volume - Handling large JSON Files can pose challenges in terms of memory usage, processing time and network bandwidth.
        - Mitigation COnsiderations for scalbility and performance implications while working with large datasets
           - Data streaming
           - Pagination
           - Compression
           - Distributed processing
             
## Common strategies for Data Quality Management 
Responsible data handling - Must have adequate regulations and policies that govern the collection use and protection of data

### Data Policies
Formal guidelines that govern how data is collected, used, managed and protected in an organisation
Ensure data is handled responsibly, ethically and in complaince to laws and industry regulations/standards

#### Data Access and usage policies
Outline who can access data and how it can be used. They specify access levels, permissions and protocols for handling sensitive or confidential information to **safeguarddata privacy and security prevent unauthorised access and ensure data is used for a legitimate business purpose**

#### Data retention and archiving policies
Outline how long data should be retained, where it should be stored and when should should it be destroyed securely or be archived

#### Data sharing policies
Govern how data is ahred with external parties i.e. partners, vendors or regulatory authrities

**GDPR - General Data Protection regulations**
Comprehensive data protection law enacted by the EU in2018.
##### Key principles are:

    - ** Lawfulness fairness and transparency ** data processing must be lawful fair and transparent
    - ** Purpose limitation ** - personal data should only be collected for the explit and specific purpose
    - ** Data minimisation ** - Only necessary data that is relevant to the purpose should be processed
    - ** Accountability and transparency ** - Data controllers are responsible for demonstrating GDPR compliance
    - ***Integrity and confidentiality*** personal data should be processed that ensures security, protection against unlawful access, or accidental loss or damage
    - ***Accuracy***Personal data should be kept accurate and up to date
    - ***Storage limitation***
    
##### Requirements

    - ***Consent*** - Organisations must obtain consent from individuals before collecting personal data
    - ***Data Subject rights*** - right to an individual to access, rectify, restrict processing, erase their data
    - ***Data Transfers*** - Regulates transfer of data outside EEA to ensure that appropriate safeguards are in place

Impact on data governance and protection practices 
Challenges obtaining and managing consent
Requirements for data portability and the right to be forgotten

### Data Validation Tools
- Data quality management platforms - Informatica Data Quality, talend Data Quality, IBM Infospere Information Analyser
- Data Profiling software- SAS Data Quality, Oracle Data Profiling
- Data Validation frameworks - Apache Griffin, Great expectations - open source validation solutions
- Continuous Data quality monitoring
    - Real time anomaly detection
    - Proactive quality assurance
    - Timely correction

### Data Lineage and unique identifiers

Refers to the lifecycle of the data from its origin, usage and movement over time.
Unique identifiers - UID - codes or numbers to uniquely identify an entity in the system

UUIDs are standardised and globally unique across different systems

## Data Testing methodologies
  - **Horizontal testing** - Integrity of data across multiple systems
  - **Rule based Testing** - Validation criteria based testing
  - **Statistical testing** - detecting deviations from expected patterns and distributions

### Testing Tools
    - Open source libraries and tools - apache griffin
      Cost effective, community support vs Limited features and require technical expertise for customisation
    - Commercial data quality tools - Informatica/Talend
      Comprehensive features, userfriendly interfaces, vendor support Vs Costly license fees, dependency on vedor for updates
    - Manual testing
      - Sampling
      - Spot checking
      - Comparison with trusted sources

# Off the job traing - Activty 1
1. What is the usability score of this dataset and is it “good” or “bad”? - 8.82 - Good
2. How is this usability score calculated? - Completeness - 100%, COmpatibility - 100%, Credibility 33%
3. What are the two credibility issues with this dataset and why are they important? - Source - unknown and update frequency -
   Understanding the lineage of data is important from a lifecycle point of view. Since the source is not known we are unsure where the data is created. Update frequency is unknown and this crucial as if this is not maintained then the data may not be accurate and may be a snapshot at a particular data and time.
4. How many columns does this dataset have? - 35
5. What is the licence for this dataset and how would you summarise the usage rights in your own words? Open Data Commons
   does not specify any usage rights related information apart from the disclaimer "Any damages resulting from its use are disclaimed."
6. what does md5 mean - MD5 (message-digest algorithm) is a cryptographic protocol used for authenticating messages as well as content verification and digital signatures. MD5 is based on a hash function that verifies that a file you sent matches the file received by the person you sent it to.
7. What are the dataTypes sc:Integer and sc:Boolean? Find an example of a Boolean field. Salary/numcompaiesworked are exmaples of integer/ Overtime yes/No is an example of boolean field
8. why does using compression aid sustainability and net-zero goals? It requires less storage space and thus will help in lesser server requirement which will mean less energy to support infrastructure and thus helping environment
9. What is the possible issue in identifying the meaning of the column named 'YearsSinceLastPromotion', especially when interpreting the value of '0' in one of the fields? - it does not provide any difference between employess who have never been promoted or have just been promoted.
10. Compare the contents of the column 'Over18' and 'OverTime', what data quality issue can you identify? - Both are Boolean value columns but the values are inconsistent and may pose problems when comparing across multiple systems.
11. What are some possible issues with the data quality of 'MonthlyIncome' and 'Monthly Rate'? -  Arent intuitive and cannot understand the cintext without underlying meta data
12. How would you validate the 'EmployeeNumber' column and what needs paying special attention to? - It should be unique(UID)/have no duplicate values. Should be generated to the next sequence number at the time the employee joins the organisation.


      
