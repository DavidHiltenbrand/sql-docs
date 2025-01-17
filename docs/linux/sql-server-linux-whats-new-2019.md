---
title: What's New for SQL Server 2019 on Linux
description: This article highlights what's new for SQL Server 2019 on Linux.
author: VanMSFT 
ms.author: vanto
ms.date: 10/23/2019
ms.topic: conceptual
ms.prod: sql
ms.technology: linux
---

# What's new for SQL Server 2019 on Linux

[!INCLUDE[appliesto-ss-xxxx-xxxx-xxx-md-linuxonly](../includes/appliesto-ss-xxxx-xxxx-xxx-md-linuxonly.md)]

This article describes the major features and services available for SQL Server 2019 running on Linux.

> [!NOTE]
> For package downloads and known issues, see the [Release notes](sql-server-linux-release-notes-2019.md?view=sql-server-linux-ver15).

## Updates

The updates have been made in SQL Server 2019 on Linux:

| New feature or update | Details |
|:-----|:-----|
|New container registry|[Get started with SQL Server containers on Docker](quickstart-install-connect-docker.md) |
|Replication support |[SQL Server Replication on Linux](sql-server-linux-replication.md)
|Support for the Microsoft Distributed Transaction Coordinator (MSDTC) |[How to configure MSDTC on Linux](sql-server-linux-configure-msdtc.md) |
|OpenLDAP support for third-party AD providers |[Tutorial: Use Active Directory authentication with SQL Server on Linux](sql-server-linux-active-directory-authentication.md) |
|Machine Learning on Linux |[Configure Machine Learning on Linux](sql-server-linux-setup-machine-learning.md) |
|`tempdb` improvements | By default, a new installation of SQL Server on Linux creates multiple `tempdb` data files based on the number of logical cores (with up to 8 data files). This does not apply to in-place minor or major version upgrades. Each `tempdb` file is 8 MB with an auto growth of 64 MB. This behavior is similar to the default SQL Server installation on Windows. |
| PolyBase on Linux | [Install PolyBase](../relational-databases/polybase/polybase-linux-setup.md) on Linux for non-Hadoop connectors.<br/><br/>[PolyBase type mapping](../relational-databases/polybase/polybase-type-mapping.md). |
| Change Data Capture (CDC) support | Change Data Capture (CDC) is now supported on Linux for SQL Server 2019. |
| Microsoft Container Registry | The [Microsoft Container Registry](https://www.ntweekly.com/2019/09/23/microsoft-container-registry-to-replace-docker-hub-for-new-images/) now replaces Docker Hub for new official Microsoft container images, including [!INCLUDE[sql-server-2019](../includes/sssqlv15-md.md)]. |
| Non-root containers | [!INCLUDE[sql-server-2019](../includes/sssqlv15-md.md)] introduces the ability to create safer containers by starting the [!INCLUDE[sql-server](../includes/ssnoversion-md.md)] process as a non-root user by default. See [build and run SQL Server containers as a non-root user](sql-server-linux-configure-docker.md#buildnonrootcontainer) for more details. |
| &nbsp; | &nbsp; |

## Next steps

To install SQL Server on Linux, use one of the following tutorials:

- [Install on Red Hat Enterprise Linux](quickstart-install-connect-red-hat.md?view=sql-server-linux-ver15)
- [Install on SUSE Linux Enterprise Server](quickstart-install-connect-suse.md?view=sql-server-linux-ver15)
- [Install on Ubuntu](quickstart-install-connect-ubuntu.md?view=sql-server-linux-ver15)
- [Run on Docker](quickstart-install-connect-docker.md?view=sql-server-linux-ver15)
- [Provision a SQL VM in Azure](/azure/virtual-machines/linux/sql/provision-sql-server-linux-virtual-machine?toc=/sql/toc/toc.json)

To see other improvements introduced in SQL Server 2019, see [What's New in SQL Server 2019](../sql-server/what-s-new-in-sql-server-ver15.md).

> [!TIP]
> For answers to frequently asked questions, see the [SQL Server on Linux FAQ](sql-server-linux-faq.md).

[!INCLUDE[get-help-options](../includes/paragraph-content/get-help-options.md)]
