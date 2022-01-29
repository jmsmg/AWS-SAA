# AWS SAA_Storage

## [S3](https://aws.amazon.com/ko/s3/)

- 출제경향
  - S3 수명 주기 관련문제
  - 

### 수명 주기

![S3_class](img/AWS-SAA_Storage_01_S3.png)

### 객체 버전 관리

- Retain Until Date
  - 객체 버전에 보관 기간을 지정함
    - 객체 버전의 메타데이터에 보존기간을 저장함
    - retain until date를 설정을 변경하고 버전 변경을 했을 때 이전버전은 그대로 유지됨

### Encryption for object(객체 암호화)
> 서버측 암호화, 클라이언트측 암호화 2가지로 나누어진다.

#### 1. 서버측 암호화

- SSE-S3
  - AWS에서 관리, S3 데이터키, **AES-256 암호화타입**, 감시, 추적 불가
- SSE-KMS
  - AWS에서 관리, KMS CMK(Customer Master Key), 감시, 추적 가능

#### 2. 클라이언트측 암호화

- SSE-C
  - 클라이언트 제공 암호화키 사용, **HTTPS 사용**, AWS에서 키를 저장하지않음
- Client Side Encryption(클라이언트측 암호화)
  - 클라이언트가 S3로 파일을 보내기전 암호화하고 S3에 보관함
