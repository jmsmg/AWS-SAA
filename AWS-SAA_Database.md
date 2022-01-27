# AWS-SAA_Database

## RDS

### 읽기 전용 복제본, 다중 AZ 배포 및 다중 리전 배포

#### [다중 AZ 배포](https://aws.amazon.com/ko/rds/features/multi-az/)
  > 고가용성이 주요 목적

- **동기식 복제**를 따르고, 단일 리전 내에 2개 이상의 가용영역에 걸쳐있음

#### [읽기 전용 복제본](https://aws.amazon.com/ko/rds/features/read-replicas/)
  > 확장성이 주요 목적

- **비동기식 복제**를 따르고, 가용 영역, 교차 AZ 또는 교차 리전 내에 있을 수 있음