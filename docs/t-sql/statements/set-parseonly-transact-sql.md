﻿---
title: "SET PARSEONLY (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: "11/27/2017"
ms.prod: "sql"
ms.prod_service: "database-engine, sql-database"
ms.service: ""
ms.component: "t-sql|statements"
ms.reviewer: ""
ms.suite: "sql"
ms.technology: 
  - "database-engine"
ms.tgt_pltfrm: ""
ms.topic: "language-reference"
f1_keywords: 
  - "PARSEONLY_TSQL"
  - "SET_PARSEONLY_TSQL"
  - "PARSEONLY"
  - "SET PARSEONLY"
dev_langs: 
  - "TSQL"
helpviewer_keywords: 
  - "parsing [SQL Server], SET PARSEONLY statement"
  - "checking syntax"
  - "PARSEONLY option"
  - "syntax [SQL Server], verifying"
  - "verifying syntax"
  - "SET PARSEONLY statement"
ms.assetid: 514ab042-c53e-4d96-be71-fb08fcc6ef3c
caps.latest.revision: 18
author: "edmacauley"
ms.author: "edmaca"
manager: "craigg"
ms.workload: "Inactive"
monikerRange: ">= aps-pdw-2016 || = azuresqldb-current || = azure-sqldw-latest || >= sql-server-2016 || = sqlallproducts-allversions"
---
# SET PARSEONLY (Transact-SQL)
[!INCLUDE[tsql-appliesto-ss2008-asdb-asdw-pdw-md](../../includes/tsql-appliesto-ss2008-asdb-asdw-pdw-md.md)]

  Examines the syntax of each [!INCLUDE[tsql](../../includes/tsql-md.md)] statement and returns any error messages without compiling or executing the statement.  
  
 ![Topic link icon](../../database-engine/configure-windows/media/topic-link.gif "Topic link icon") [Transact-SQL Syntax Conventions](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## Syntax  
  
```  
  
SET PARSEONLY { ON | OFF }  
```  
  
## Remarks  
 When SET PARSEONLY is ON, [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] only parses the statement. When SET PARSEONLY is OFF, [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] compiles and executes the statement.  
  
 The setting of SET PARSEONLY is set at parse time and not at execute or run time.  
  
 Do not use PARSEONLY in a stored procedure or a trigger. SET PARSEONLY returns offsets if the OFFSETS option is ON and no errors occur.  
  
## Permissions  
 Requires membership in the **public** role.  
  
## See Also  
 [SET Statements &#40;Transact-SQL&#41;](../../t-sql/statements/set-statements-transact-sql.md)   
 [SET OFFSETS &#40;Transact-SQL&#41;](../../t-sql/statements/set-offsets-transact-sql.md)  
  
  
