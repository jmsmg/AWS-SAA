# AWS-SAA Networking, Content Delivery

## [Tran-sit Gateway](https://aws.amazon.com/transit-gateway/)
  > Amazon Virtual Private Cloud(VPC)와 온프레미스 네트워크를 단일 게이트웨이에 연결할 수 있도록 하는 서비스

## [API Gateway](https://docs.aws.amazon.com/ko_kr/apigateway/latest/developerguide/welcome.html)

- 상태저장(WebSocket)
- 상태비저장(HTTP, REST)

## [Direct Connect](https://aws.amazon.com/ko/directconnect/)
  > 병목현상 방지

- 온프레미스에서 AWS로 물리적인 연결을 함
- 연결까지 시간이 오래걸림

## [Global Accelerator](https://docs.aws.amazon.com/ko_kr/global-accelerator/latest/dg/what-is-global-accelerator.html)

- 글로벌 트래픽이 최적의 엔드포인트로 연결되도록 지연시간을 줄여주는 서비스

### Global Accelerator vs Cloud Front
  > 두 서비스 모두 DDoS 공격을 막기 위해 AWS Shield와 통합되어 있음

- CloudFront는 캐시 가능한 콘텐츠(이미지, 비디오)와 동적인 콘텐츠(API 가속화 및 동적 사이트 제공)의 성능을 모두 개선

- Global Accelerator는 엣지에서 패킷을 단일 또는 여러 AWS 리전에서 실행되는 애플리케이션
  - 게임(UDP), IoT(MQTT), VoIP, HTTP 사용 사례에 적합