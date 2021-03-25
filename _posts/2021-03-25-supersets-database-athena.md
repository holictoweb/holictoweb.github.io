---
title: "apache superset athena database 연결"
date: 2021-03-20 08:26:28 -0400
categories: superset athena database connect
---


## superset database 설정

- Data > databases 선택 -> + 버튼 click (Add a new record)

> superset 에서 연결 가능한 DBMS drivers 정보 
>   > https://superset.apache.org/docs/databases/installing-database-drivers

- athena 연결을 위해 사용 가능한 driver는 두 종류
  - pip install "PyAthenaJDBC>1.0.9 
  - pip install "PyAthena>1.2.0
