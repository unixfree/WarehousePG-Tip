# WHPG 교육 목차

## 참고 URL
```
https://warehouse-pg.io/docs/7x/
https://gpdbkr.blogspot.com/
```

1. 아키텍처 설명
2. 설치 <br>
   gpinitsystem <br>
   gpdeletesystem <br>
   gpinitstandby <br>
   gpactivatestandby <br>
   gpstart -a <br>
   gpstop -u | -af <br>
   gpstate -e | -m  | -s  <br>
3. table 생성
   - 분산키
   - 파티션
4. external table 생성
5. 데이터 적재
   gpload, gpfdist
6. PXF
   pxf 
7. TPC-DS 수행
8. 백업/복구
   gpbackup/gprestore
9. 노드장애 복구 
   gprecoverseg
10. 운영관리
   > 카달로그 무결성 확인 : gpcheckcat
     gpcheckcat -g /home/gpadmin/fix_catalog.sql testdb
   > vacuum, analyze, reindex
   > skew 관리.
11. 자원관리
    Resource Group
12.
    gpconfig
13. 기타
    hint
