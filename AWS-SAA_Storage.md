# AWS SAA_Storage

## S3

### [Encryption for object(객체 암호화)](https://docs.aws.amazon.com/ko_kr/AmazonS3/latest/userguide/UsingEncryption.html)
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
