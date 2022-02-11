# AWS-SAA_Database

## RDS

### 읽기 전용 복제본, 다중 AZ 배포 및 다중 리전 배포

#### [다중 AZ 배포](https://aws.amazon.com/ko/rds/features/multi-az/)
  > 고가용성이 주요 목적

- **동기식 복제**를 따르고, 단일 리전 내에 2개 이상의 가용영역에 걸쳐있음

#### [읽기 전용 복제본](https://aws.amazon.com/ko/rds/features/read-replicas/)
  > 확장성이 주요 목적

- **비동기식 복제**를 따르고, 가용 영역, 교차 AZ 또는 교차 리전 내에 있을 수 있음

## DynamoDB

### DynamoDB Accelerator(DAX)
  > elastic cache와 비교하는 문제

- 완전 관리형 고가용성 인메모리캐시로 최대 10배 성능

## Elastic Cache
  > 캐싱 패턴 지정가능해야함(개발업무 추가), 오류 node 발견시 자동 recover

### Cache Engine

- Memcahed
  - write와 read를 in-memory할 수 있도록 처리
  - 탄력적으로 clust가 증가하고, 감소할 수 있게 관리되며, unique key를 통해 blob처럼 사용 가능

- Redis
  - Memcached보다 strings, list, set의 데이터 타입 특화된 cache 서비스
  - Memcached와 달리 in-memory data를 disk에 유지 할 수 있는 기능이 있음

### Elastic Cache vs DynamoDB Accelerator(DAX)

- Elastic Cache는 집약된(aggregated) 결과를 캐싱
- DAX는 DB 결과 각각의 오브젝트를 캐싱