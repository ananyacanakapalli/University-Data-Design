# University-Data-Design-Project

Problem Background:
You are part of the data analytics and architecture team that oversees “all data” for a big university
that provides on-campus as well as online courses. Your team processes thousands of students 
and hundreds of cohorts every year.

As the University has added more courses, such as professional development, certificates, and
only online courses, handling growth (and the data) has become more critical. 
The University has current solutions and data architecture based on archaic infrastructure
creating a mix of applications and data stores on the cloud and on-premise data centers. Some 
vendor applications use the cloud and then sync the data, and some use the University’s data 
center. The data center is becoming challenging to manage, and the Chancellor’s office is facing 
multitudes of problems in reconciling data and figuring out a single source of truth for reporting
and advanced analytics use cases.

In the last ten years, many universities in the same geography and space have moved to the 
cloud and started looking at data (irrespective of the domain- student, employee, course, etc) as 
an asset.

Current data analytics architecture is built in hybrid mode (part cloud + part on-premises) and 
patched regularly. However, the University spends a significant budget on maintaining old data 
sources and integrations. Hence, releasing new features quickly or analyzing data is a 
significantly cumbersome activity. In addition, the University is in the hyper-growth stage after the 
pandemic, where they have launched many online degrees, courses, and certificate programs to 
attract more students globally; these programs have become immensely popular due to the
University’s brand value in the higher education space.

With ever increasing growth targets, new courses, and accompanying heavy enrollment to the
online courses several challenges have emerged, such as, but not limited to, varied data 
processing techniques and technologies, people, processes, data governance, and mainly 
different representations/models of a student, employee and curriculum data effectiveness. All of 
which contribute to the chaos in reaching to the single source of truth.

The Chancellor’s office is very interested in also using predictive analytics methods and AI across 
all critical data sets where the University, faculty, and staff should be able to identify and help 
support students in need. But as the data is scattered across all the infrastructure (data silos), it 
is utmost difficult to think about such advancements practically. 

The Chancellor’s office wants to solve the duplication in data reporting. In addition, they would 
like to facilitate more data standardization across their colleges so that you will get a uniform 
picture of students and staff and their achievements, successes/challenges, involvements, etc. 
While doing that, data security is of utmost importance, along with the scale of acquiring and
processing the data. 

The current in-house data warehouse system is overwhelmed, and the cost of maintenance, 
enhancements, and upgrades is too high, impeding the business team from rapidly introducing 
new products. There is no standardization or reporting tools either. Due to the archaic
infrastructure and processes, the University cannot process unstructured or semi-structured data 
and only base the decisions and insights on structured data, which does not comprise more than 
50% of activities on-campus or online for staff and students. A major opportunity is lost there.
Your team is tasked to choose the appropriate cloud infrastructure and data platform and ensure
the creation of a data migration and management strategy. The standard data retention period is 
25 years for online reporting of student data. The data team is also responsible for creating a data 
retention policy that will help the university staff and students with an acceptable SLA structure
and keep the cost of storage in perspective.

The Chancellor’s office has also asked if your team is building a unified data analytics approach 
to support various internal and external teams for different use cases. Examples of such use
cases include but are not limited to at-risk students (dropouts, failures, financial or similar 
hardship), compliance monitoring and reporting, gauging effectiveness of staff and curriculum,
various levels, and types of segmentation for student services/counselor organizations, 
sales/marketing insights and alerts, and student/staff 360 view-related use-cases. This unified 
data architecture would also be the single source of truth for all regulatory Reports. The data team 
will also provide the Chancellor’s Office with data Governance processes and KPIs. 

In summary, the University is interested in implementing a common data platform to improve its 
operational and analytical infrastructure. Your team is tasked to identify and implement the 
following: 

A common data management platform to enable data sharing and manage the flow of 
data from business applications/data sources and out to data consumers—applications, 
processes, and business units. Key Data Management Platform capabilities: 

Seamless Data Integration: Support data integration methods ranging from daily
syncs through change data capture/movement of data to more real-time data 
integration methods such as web services and the use of APIs to manage the flow 
of data from business applications/data sources and out to data consumers. 

Single source of truth: Provide one golden copy of data to consumers with data 
governance controls with established data quality, lineage, security, and privacy 
standards. 

Master Data Management and Metadata repository version control: Enable 
continuous access and processing of metadata to attain visibility across 
institutional data, for both technical and business staff, to increase the value of the 
University’s data and drive business outcomes. 


A unified data store for traditional and advanced Analytics (data warehouse, data lake, 
lake house) that scales the University’s reporting and analytics capabilities. Key Data 
Store for Analytics capabilities should include, but not limited to: 
o Data Analytics Governance: Provide data analytics governance controls to 
improve data security, quality, and consistency for institutional decision-making and 
key business metrics to achieve desired business outcomes. 
o Analytical Data Models: Accelerate the development of analytical data models to 
enable data-driven decision-making at all operational levels, drive innovation, and 
realize business value faster. 
o Predictive analytics and Artificial Intelligence oriented use-case incubation:
Provide the ability to dynamically identify and support new use cases and analysis 
through artificial intelligence. 
Assumptions: 
You can assume that data flowing to the current data warehouse is from various database 
systems. Therefore, the source systems and their database system-related standardization 
changes are not in the scope of this redesign. 
Such upstream systems have the following databases and messaging systems from which 
transactions and events originate, e.g., MySQL, Oracle, Cassandra, SQL server, Kafka, 
PostgreSQL, ActiveMQ, etc. From the cloud perspective, you will also review data from Amazon 
S3, Redshift, salesforce, etc. 
You will also need to support batched and streaming data originating from various sources, such 
as ERP, CRM, LMS systems, mobile apps, and so on. 
To optimize costs, your data lake/lake house/ data warehouse must support historical and 
incremental data models and storage requirements.
Your data design will be accessed via microservices by downstream reporting or business
systems via developers from various business teams, finance, analysts, and data scientists. 
Your goal is to establish a design for: 
1. Unified data access and storage 
2. Prepping data for downstream processes, removing irregularities in data.
3. Scalable data ingestion and extraction 
4. Data security
5. Easy of hooks for integration 
6. Optimal storage usage for different use cases
7. Cost efficiency without reducing the Effectiveness of the use cases.
8. Scalability in overall design to accommodate future business growth.
