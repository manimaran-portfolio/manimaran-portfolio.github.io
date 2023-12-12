## Python Developer | Test Automation Engineer | Cloud Practitioner

# Professional Summary

I am a Python developer with 8 years of experience in automation development and testing, data analysis, and cloud engineering. I have successfully delivered innovative solutions for leading banking clients such as CitiBank and Morgan Stanley, using cutting-edge technologies and frameworks. I am seeking a challenging opportunity to apply my skills and expertise in a dynamic and collaborative environment.

# Technical Skills

- **Programming Languages**: Python, Java, SQL, Shell scripting
- **Web Development**: Flask, FastAPI, HTML, CSS, jQuery
- **Data Analysis**: Pandas, PySpark, Hadoop, Hive, HBase
- **Testing**: Selenium, Cucumber, Pytest, Xray, Jira
- **Cloud**: AWS, Docker, Jenkins
- **Version Control**: Git
- My GitHub Repositories: [Github](https://github.com/manimaran990)
- Hacker-rank profile: [HackerRank](https://www.hackerrank.com/m4n1g)

# Professional Experience

## Infosys - Morgan Stanley, Montreal CA - Python Developer
OCTOBER 2019 - NOVEMBER 2023
- Engineered a robust connectivity dashboard using FastAPI and Flask, enabling the Exchange Connectivity team to concurrently manage multiple jobs seamlessly.
- Designed a Single Page Application for the SIFMA web application, streamlining disaster recovery testing, IP connectivity, order sending/fetching logs, and report generation.
- Developed a regression framework to execute regression tests and replay exchange messages, resulting in a notable 40% performance improvement for enhanced testing efficiency.
- Spearheaded the development of a pivotal internal project as part of the Xray team, involving the collection and transformation of Jira data from various sources.

## Infosys - Morgan Stanley(Offshore), India - Python Developer
SEPTEMBER  2018 - OCTOBER 2019

- Did data collection/cleaning on jira data from multiple data sources, used by high level managers using tableau dashboard.
- Used python for extraction and cleaning of raw data of multiple types like excel, streaming and flat file format.
- Automated execution of ETL process using jenkins pipeline, written unit tests using pytest and testplan framework.
- Designed and maintained a FastAPI-based web service for Xray and Jira integration, serving as a test manager service.
- These services are multiple internal teams to automate their tests/test execution and maintained jira sanity for those respective projects.

## Infosys - CitiBank Client, Chennai India - Technology Engineer
DECEMBER 2015 - SEPTEMBER  2018
- Implemented shell and Python scripts, leading to an impressive 80% reduction in data cleansing time for the payment insights project.
- Developed various tools and automation solutions using Python and shell scripting, contributing to the efficiency of the Citi-digitization project.
- Gained hands-on experience in the Hadoop ecosystem, optimizing the big data ETL process by 40% through effective performance tuning methods.
- Engineered a robust regression framework leveraging Python, automating data validations across multiple project layers.
- Demonstrated expertise in testing by implementing comprehensive test coverage and unit tests using Python frameworks.

# Education

- Masters in Computer Applications (MCA) - College of Engineering Guindy, India (2015)

# Certifications

<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="42212cde-2a66-49d1-bc36-db7ce86a8d71" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="fb5a8646-cd28-408f-ab43-a7d4272e4798" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="3aa31656-37d1-4466-ba3f-ae2334bdb450" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="852d2d50-5ab1-43e0-ae96-6fbe211cdfdc" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="1baa609f-b7b6-4cc1-a184-9ef182203540" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>
<div data-iframe-width="150" data-iframe-height="270" data-share-badge-id="c2b129c2-5ca8-4b6f-a4ed-d8c7911f1a8b" data-share-badge-host="https://www.credly.com"></div><script type="text/javascript" async src="//cdn.credly.com/assets/utilities/embed.js"></script>

# Client/Infosys Specific Tools/Technology:
**Ingestion Testing Tool (Citi Client):** Extracting the data from various product processors and getting the records from hbase for the validation purpose is a tedious task. The Citi Digitization project has lots of product processors and new product processors are onboard frequently. For the validation as well as regression purpose he created a generic framework with UI to efficiently extract the data and convert them into json format and generate a report in excel with a detailed break report summary.
- **Need for this tool:**  Doing regression and functionality tests on a large dataset and frequency of running those tests manually is challenging. This framework overcomes this problem.
- **Its benefits**:
- The Ingestion Testing tool has reduced test reporting effort from 40 minutes to 2 minutes on a daily basis for the client for each Product processor.
- It has a simple UI with various selection options to generate the reports.
- Faster data retrieval using row prefix filtering the hbase records for the data validation.
- Can be able to validate 1M records with >300 columns within 3 mins in cluster mode.

**Payment Tracker Tool (Citi Client):**
Transactions initiated by the client will be flown through many components including various big data tools like kafka, hbase and ignite layers. This utility will help us to find whether all the components are up and running and check the transaction if it got stuck in the middle of the process and to investigate the reason for it. This framework was developed in Java.
- **Need for this tool:** Tracking a payment manually in multiple components is a tedious task. This will overcome this issue.
- **Its benefits:**
- Environment readiness test requires any of the members from all the environments to ensure whether it’s up or not. This tool helped us to eliminate this dependency and as well as we can use it to check for the readiness of all the components within 1 minute of time.
- This tool was used by the ERT (Environment Readiness Test) team on a daily basis before initiating payments for all the product processors.

**Exchange Connectivity Dashboard (MS client):**
The Exchange connectivity team is a part of algo-trading. They are the communication bridge between the algo-engines and the actual stock exchanges. Those exchanges are controlled by exchange instances. Main functionality of these exchanges is to send fix-messages to exchanges and get back their response (to fill/ack/cancel the order). I have helped the team to create a SPA dashboard to maintain control of those exchange instances in a single place using FastAPI, flask for backend and jquery, js, css for front-end.
- **Need for this tool:** Previously multiple CLI tools were used to achieve various tasks such as sending fix messages, view logs, netadmin, check status, etc. Which is not a beginner friendly and tedious while copy, pasting message. This web-based dashboard made these redundant tasks more accessible and user friendly.
- **Its benefits:**
- Single point of access to control those exchange instances.
- Can be used to check status, restart the instance, send fix messages, view logs, perform netadmin commands on those exchanges.


# PERSONAL PROJECTS:
**Expense Manager:**
Developed a Django-based money tracking app automating expense management. Offers spending analysis, insights, and AI-driven suggestions with Language Model (LLM) technology. Demonstrates expertise in web development, data analysis, and AI integration.
Project link: [expenseTracker](https://github.com/manimaran990/expenseTracker)

**Second Brain:** 
Innovated a user-friendly note-taking app with ChatGPT-like interface.
Supports various formats (URLs, YouTube links, images, Markdown) and features Chrome plugins and a Telegram bot for added convenience.
Utilizes LLM models for intelligent categorization, showcasing proficiency in natural language processing and AI-driven classification.
Project link: [Second Brain](https://github.com/manimaran990/secondBrain)

