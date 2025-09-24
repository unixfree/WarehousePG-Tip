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
   gpstop -u | -af 
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
8. TPC-DS 수행
9. 백업/복구
   gpbackup/gprestore
10. 노드장애 복구 
   gprecoverseg
11. 운영관리
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
