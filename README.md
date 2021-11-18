# 북스토어 전자상거래 서비스

## 서비스 목표
* 북 스토어 전자 상거래 서비스 구축
    - 스프링 클라우드 기반 MSA 서비스 기술 습득
    - Service Mesh 내 디스커버리와 API 게이트웨이 구축을 통한 마이크로서비스 라우팅과 로드벨런싱, 인증 기술 습득
    - Kafka를 활용한 서비스 간 데이터 통신
    - RestTemplate를 활용한 서비스 호출
    - 도커와 도커 컴포즈를 활용한 클라우드 환경의 서비스 배포 및 운영 환경 구축

## 서비스 아키텍처 구성도
![서비스구조도 drawio](https://user-images.githubusercontent.com/32921225/142336641-ddaaec33-abf1-49f1-b5a2-b3603da1e080.png)

## 팀
* **팀명**: One More Things
* **팀원**
    - **민웅기** [팀장]
        - 프로젝트 총괄
        - Catalog Service 담당
    - **오지웅**
        - Order Service 담당
    - **신혜원**
        - 디자인 총괄
        - User Service 담당
    - **김남곤**
        - User Service 담당


## 요구사항
- Spring Boot Swagger를 통한 API Doc 생성
- 사용자 등록/인증
- 사용자) 상품 조회, 상세보기, 장바구니, 구매하기, 결제하기, 주문 상품 조회, 각 목록의 페이징 처리
- 관리자) 사용자의 기능 + 상품 등록 + 주문 된 상품 상태 변경 + 결제 내역 확인
- Backend) Spring Boot + Spring Cloud + Kafka 사용 
- Frontend) React 사용

## 프로젝트 진행 과정
0. 조별 프로젝트
1. 요구사항 정의서 작성
2. 기능 명세서 작성
3. 사용자 시나리오 또는 유스케이스 작성
4. API 설계서 작성 
    - RESTful API
    - GET/POST/PUT/DELETE 구현 
        - 전체 조회, 개별 조회 (by ID, Date, Keyword)
5. 기능 구현
6. 간단한 UI 추가 
7. 모듈 프로젝트 마지막
    - 도커 이용해 서비스 컨테이너화, AWS로 Migrate 작업 (EC2 + RDS)
