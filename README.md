# Azure Database Migration
### By Spyridon Manouras
Email: spirosmanu@gmail.com  
Started on: 23/01/2024

## Project Overview
This project showcases the architectural and implementation skills in cloud-based database systems on Microsoft Azure. The primary objective is to establish a production environment database and migrate it to Azure SQL Database, demonstrating cloud engineering expertise.

## Current Progress
### Initial Setup
- **Virtual Machine Setup**: Established a Windows Virtual Machine (VM) on Microsoft Azure to serve as the cornerstone of the production environment. This VM emulates the functions of a Windows server, replicating the operations of an on-premise system within a company.
- **Network Configuration and Firewall Rules**: Configured the appropriate network settings and firewall rules to establish a connection to the VM using the RDP protocol.
- **Remote Connection**: Initiated a remote connection to the VM using Microsoft Remote Desktop and the RDP protocol, providing direct access to the VM's operating system for efficient management and configuration.
- **SQL Server Installation**: Installed SQL Server and SQL Server Management Studio (SSMS) on the VM. These tools are crucial for proficient database management and mirror the capabilities of a corporate database server.
- **Production Database Creation**: Created the production database by restoring from a backup file of the AdventureWorks database. This sample database emulates a fictional manufacturing company's operations, including various tables, views, stored procedures, and a diverse dataset.

### Recent Developments
- **Database Connectivity**: Successfully established connections to both the local SQL Server (Windows) and the Azure SQL Database using Azure Data Studio.
- **Schema Comparison and Migration**: 
  - Utilized the SQL Server Schema Compare extension in Azure Data Studio for schema comparison.
  - Completed schema comparison, highlighting differences between the local SQL Server database and the Azure SQL Database.
- **Data Migration**:
  - Leveraged the Azure SQL Migration extension within Azure Data Studio.
  - Executed the data migration process from the on-premise database to the Azure SQL Database. The steps included:
    1. **Initiating Migration**: Through Azure Data Studio, the migration process was initiated by selecting the source (local SQL Server) and the target (Azure SQL Database).
    2. **Migration Validation**: Performed a preliminary validation check to identify any potential issues before the actual data transfer.
    3. **Data Transfer**: Executed the migration, transferring schema and data from the on-premise database to the Azure SQL Database.
    4. **Post-Migration Validation**: Conducted a thorough validation post-migration to ensure data integrity and completeness.

## Key Technologies Used
- Microsoft Azure
- Windows Virtual Machine
- SQL Server
- SQL Server Management Studio (SSMS)
- Microsoft Remote Desktop
- RDP Protocol
- Azure Data Studio
  - SQL Server Schema Compare extension
  - Azure SQL Migration extension

## Verification of Migration
To confirm the success of the database migration process, a comprehensive validation was carried out. This included:
- **Data Integrity Checks**: Ensuring that all data was accurately migrated without any loss.
- **Schema Validation**: Confirming that the database schema in the Azure SQL Database mirrors the original on-premise schema.
- **Configuration Review**: Verifying that all database configurations and settings are correctly implemented in the Azure environment.
- **Performance Testing**: Conducting tests to evaluate the performance and responsiveness of the migrated database under typical load conditions.

The successful completion of these validation steps assures that the database migration upholds the principles of data integrity and operational continuity in its new cloud environment.
