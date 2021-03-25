---
title: "apache superset athena database 연결"
date: 2021-03-20 08:26:28 -0400
categories: superset athena database connect
---


#### superset database 설정

- Data > databases 선택 -> + 버튼 click (Add a new record)

> superset 에서 연결 가능한 DBMS drivers 정보 
>   > https://superset.apache.org/docs/databases/installing-database-drivers

- athena 연결을 위해 사용 가능한 driver는 두 종류
  - PyAthenaJDBC
    + pip install "PyAthenaJDBC>1.0.9 
    + JDK 8+
    - awsathena+jdbc://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com/
  - PyAthena
    - pip install "PyAthena>1.2.0
    - awsathena+rest://{aws_access_key_id}:{aws_secret_access_key}@athena.{region_name}.amazonaws.com/

> superset 최신 버젼에서는 databases 연결 후 datasets 연결 시 스키마 정보를 추가 하기 때문에 위의 connection string 에서는 별도의 스키마 지정은 필요 없음

