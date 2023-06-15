# Document Export Application

## Description
Export application to retrieve documents from FileNet Content Engine based on provided document class and the range of date created. 

## Table of Contents
- [Prerequisites](#Prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Prerequisites
1. Java Runtime 1.8 or above. 
2. Connectivity to the FileNet CPE server from the machine where the application would be executing. 
3. Sufficient storage on the local server for downloading the files. 

## Installation
Unzip the contents of the zip file into a local directory.
For Windows based servers please use C:\ drive to use the application with default setting.	

Configuration of the application is stored in application.properties. 
A sample file with description for each property is included in the package. 
Please edit this file to change FileNet connection related parameters. 
Also, please change the Document Class and the date range for which export is required. 
It is recommended to not to use extremely large date ranges to avoid out of memory exceptions. 

Log related configurations are present in logback.xml. Please edit line number 11 for changing log file location and name. 
To change log level, change the same in line number 18. 

## Usage
Execute the application using following command from the same location where jar file is present: 
Java -jar <name of the jar file>
Please see the screenshot of the sample execution in the document named: DocumentExport-Sample Execution Documentation.docx

## License
Licensed to be used for demo purpose. 