# AWS-SAA Networking, Content Delivery

## [Global Accelerator](https://docs.aws.amazon.com/ko_kr/global-accelerator/latest/dg/what-is-global-accelerator.html)

- 글로벌 트래픽이 최적의 엔드포인트로 연결되도록 지연시간을 줄여주는 서비스

### Global Accelerator vs Cloud Front
  > 두 서비스 모두 DDoS 공격을 막기 위해 AWS Shield와 통합되어 있음

- CloudFront는 캐시 가능한 콘텐츠(이미지, 비디오)와 동적인 콘텐츠(API 가속화 및 동적 사이트 제공)의 성능을 모두 개선

- Global Accelerator는 엣지에서 패킷을 단일 또는 여러 AWS 리전에서 실행되는 애플리케이션
  - 게임(UDP), IoT(MQTT), VoIP, HTTP 사용 사례에 적합