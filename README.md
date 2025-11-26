## WHPG 교육 목차

### 참고 URL
```
https://warehouse-pg.io/docs/7x/
https://gpdbkr.blogspot.com/
```

1. 아키텍처 설명
2. DB 설치 / 시작 / 종료 / 삭제
   ```
   gpinitsystem 
   gpdeletesystem 
   gpinitstandby 
   gpactivatestandby 
   gpstart -a 
   gpstop -u | -r |  -af 
   gpstate -e | -m  | -s  
   ```
4. table 생성
   - 분산키
   - 파티션
5. external table 생성
6. 데이터 적재
   gpload, gpfdist
7. PXF
   pxf 
8. TPC-DS 수행 <br>
9. 백업/복구 <br>
   gpbackup/gprestore <br>
11. 노드장애 복구  <br>
   마스트(Coordinator) 노드 HA : https://github.com/unixfree/whpg_coordinator_ha <br>
   세그먼트(Segment) 노드 HA : gprecoverseg -F(full) / -r(role change) <br>
12. 운영관리 <br>
    카달로그 무결성 확인 <br>
    ```gpcheckcat -g /home/gpadmin/fix_catalog.sql testdb``` <br>
   vacuum, analyze, reindex <br>
   skew 관리. <br>
13. 자원관리 <br>
    Resource Group
14. 파라메터 변경. <br>
    ```gpconfig -s max_connections``` <br>
    ```gpconfig -c statement_timeout -v 600000``` <br>
    ```gpconfig -c work_mem -v "256MB"``` <br>
15. Array, ROW_NUMBER, RANK,CTAS, Replication Table 예시 <br>
16. PL/R, PL/python 예시 <br>
17. Madlib 예시 <br>
99. 기타 <br>
    hint
