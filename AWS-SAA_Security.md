# AWS-SAA Security, Identity, & Compliance

## [IAM](https://docs.aws.amazon.com/iam/)

### 권한 경계

- 권한 경계를 설정하면 과도한 권한을 가진 사용자의 권한을 제한할 수 있음

## [AWS WAF]
- ALB, API Gateway, CloudFront에서만 사용
- Layer 7 (HTTP)
- 초당 몇번 요청 보낸지로 DDOS를 막음
 
## [AWS Shield]
- standard
  - SYN/UDP 반사공격을 막아줌

- advanced
  - DDOS 막아줌
  - 조직당 월 3000 달러

## Amazon SSM Parameter store
- 암호화 목적으로 secret key가 있을 때 시간 지남에 따라 추적이 가능 

## Amazon CloudHSM(KMS와 구분 잘해야함)

## Amazon Macie
- 지능형 탐지(머신러닝)로 민감한 데이터를 발견하고 보호함(개인정보 PII)

- ex) S3 버켓에 개인정보가 있으면 Macie가 검사하고 Cloud Watch event

## [Amazon GuardDuty](https://aws.amazon.com/ko/guardduty/)
  > 지능형 위협탐지(머신러닝)로 무단활동 차단 워크로드에서 악의적 활동을 모니터링하고, 상세한 보안 결과를 제공

- 지원소스
  - VPC 흐름 로그, DNS 로그, CloudTrail 이벤트
  - 로그 데이터 머신러닝 학습

- 서비스 비활성화시
  - 검색결과 및 구성 등의 모든 데이터가 삭제됨

## [Cognito](https://aws.amazon.com/cognito/)

### [사용자 풀 및 자격증명 풀](https://aws.amazon.com/ko/premiumsupport/knowledge-center/cognito-user-pools-identity-pools/)

- 사용자 풀(user pool) : 인증 관련
  - 앱을 위한 가입 및 로그인 웹 페이지 설계
  - 사용자 데이터 액세스 및 관리
  - 사용자 장치, 위치 및 IP 주소를 추적하고 여러 위험 수준의 로그인 요청에 대응
  - 앱에 사용자 지정 인증 흐름 사용

- 자격증명 풀(identity pool) : 액세스 제어 
  - 사용자에게 Amazon Simple Storage Service(Amazon S3) 버킷 또는 Amazon DynamoDB 테이블과 같은 AWS 리소스에 대한 액세스 권한 부여
  - 인증되지 않은 사용자를 위한 임시 AWS 자격 증명 생성 

## [Amazon Inspector](https://st-soul.tistory.com/21)
  > 자동 보안평가로 취약점 및 노출에 대비(컴퓨터로 치면 백신 검사정도?)

## [보안그룹 vs ACL](https://aws.amazon.com/ko/premiumsupport/knowledge-center/connect-http-https-ec2/)

- 보안그룹은 상태 저장 (인바운드를 하면 자동으로 아웃바운드도 OK)

- ACL은 상태 비저장