Adventureworks_OLTP_OLAP-
# SSIS Deployment and Scheduling Project
This project demonstrates deployment and automation of SQL Server Integration Services (SSIS) packages to manage and execute a typical staging routine for a data warehouse. Using AdventureWorks OLTP and OLAP databases as the foundation, this project focuses on automating the Extract Lifecycle of data warehousing through SSIS and SQL Server Agent.
## Project Overview

In this lab-based project, we:
1. Deployed an SSIS project to SQL Server's Integration Services Catalog.
2. Configured a SQL Server Agent job to automate the execution of a master extract package on a scheduled basis.
3. Captured job execution logs and lineage table data to verify the successful operation of the deployed SSIS packages.

The lab objectives align with real-world scenarios of automating ETL (Extract, Transform, Load) operations, ensuring a seamless data flow into a data warehouse.
## Features

### SSIS Deployment
- **Integration Services Catalog Setup:** Initialized `SSISDB` and created a custom folder, `YourFullName_AW`, within the catalog.
- **Project Deployment:** Deployed the SSIS project containing multiple packages designed for data extraction.

### Automation with SQL Server Agent
- **Job Scheduling:** Set up a SQL Server Agent job to execute the `Master-Extract` package weekly.
- **Execution Monitoring:** Configured log capture and history tracking for the deployed SSIS job.

### Data Verification
- **Lineage Table Logging:** Verified the execution timestamps and inserted data records in the data warehouse's lineage table to confirm successful ETL execution.



## Installation and Setup

### Prerequisites
- SQL Server Developer Edition installed and configured.
- Restored databases:
  - `AW_DW_Demo.bak` (OLAP)
  - `AW_OLTPDemo.bak` (OLTP)
- Visual Studio with SQL Server Data Tools (SSDT).

## License
This repository is licensed under the [MIT License](LICENSE).

## Acknowledgments
This project was completed as part of a data warehousing course, leveraging the AdventureWorks datasets. 
Developed by: Dhaval Tailor
Course: PROG 1830 Data Warehouse Fall 2024
Instructor: Marsha Baddeley
