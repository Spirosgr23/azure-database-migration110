# Azure SQL Database Project Documentation

## Project Overview

This documentation outlines the comprehensive steps taken to architect and implement a secure, cloud-based database system on Microsoft Azure. It encapsulates the entire process from initial setup to integration with Microsoft Entra ID, emphasizing the strategic implementation of geo-replication and failover procedures.

## Initial Setup and Configuration

We started by establishing a foundational environment that would serve as the backbone of our database operations:

- **Virtual Machine Deployment**: Provisioned a Windows Virtual Machine (VM) on Microsoft Azure designed to replicate the role of a primary server akin to an on-premise setup.
- **Network Configuration**: Meticulously configured network settings and established firewall rules to facilitate secure connections via Remote Desktop Protocol (RDP).
- **Database Tools Installation**: Deployed SQL Server and SQL Server Management Studio (SSMS) on the VM to furnish a robust suite of management tools for our database.
- **Database Restoration**: The production database was reconstituted from a backup of the AdventureWorks sample database, thus ensuring the availability of a comprehensive dataset for subsequent tasks.

## Data Backup and Restoration Journey

Our commitment to data integrity led us to implement a rigorous backup regimen:

- **Maintenance Plans**: Implemented SSMS Maintenance Plans for systematic and regular backups, thus ensuring data was consistently safeguarded.
- **Azure Blob Storage**: Leveraged the robust and secure Azure Blob Storage to store backup files, providing redundancy and protecting against potential data loss scenarios.
- **Restoration Validation**: Demonstrated the reliability of our backup process by seamlessly restoring the production environment onto a development VM, validating the backup's efficacy.

## Geo-Replication and Failover Strategy

To ensure business continuity and data availability, we structured a geo-replication and failover strategy:

- **Geo-Replication Configuration**: Established geo-replication for our primary Azure SQL Database situated in the US East 2 region, with a synchronized secondary replica located in the US West 2 region.
- **Planned Failover Execution**: Simulated real-world disruptions by conducting a planned failover to the secondary replica, affirming the database's resilience and the smooth transition of operations.
- **Failback Procedure**: Completed the resilience testing cycle by performing a failback to the primary region, thus reinstating the original database service configuration.

## Microsoft Entra ID Integration

Embracing modern access management solutions, we integrated Microsoft Entra ID to enhance security and user experience:

- **Identity Management**: Seamlessly integrated Microsoft Entra ID to manage user access to the Azure SQL Database, moving beyond traditional authentication methods.
- **Role-Based Access Control**: Configured distinct role definitions and established both admin and reader accounts, effectively delineating access control within the database environment.
- **User Experience and Security**: By adopting Microsoft Entra ID, we not only streamlined user management but also fortified our database against unauthorized access, leveraging features like Multi-factor Authentication (MFA) for an enhanced security posture.

## Architectural Summary and Diagram

The architecture of our Azure SQL Database project is visually summarized in the following UML diagram, providing a clear depiction of the components and their interactions within our cloud-based database system.

![AZURE UML Diagram](https://github.com/Spirosgr23/azure-database-migration110/blob/main/Azure%20Project%20Diagram.jpeg)


## Conclusion

This README serves as a comprehensive record of the project, detailing each phase from initial configuration to the integration of cutting-edge identity management solutions. It stands as testament to our dedication to creating a resilient, secure, and efficiently managed database environment in Azure.

