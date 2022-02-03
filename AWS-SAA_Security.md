# AWS-SAA Security, Identity, & Compliance

## [IAM](https://docs.aws.amazon.com/iam/)

### 권한 경계

- 권한 경계를 설정하면 과도한 권한을 가진 사용자의 권한을 제한할 수 있음

## [Amazon GuardDuty](https://aws.amazon.com/ko/guardduty/)
  > 지능형 위협탐지로 무단활동 차단 워크로드에서 악의적 활동을 모니터링하고, 상세한 보안 결과를 제공

- 지원소스
  - VPC 흐름 로그, DNS 로그, CloudTrail 이벤트

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