# 식도랑

- 목적 : 음식점 기반 여행 기획 및  추천 플랫폼
- 개발 기간 : 20.08.31 ~ 20.10.08 (6주)
- [프로젝트 소개영상](https://www.youtube.com/watch?v=ayQKOBrM5lM)



## 목차

- [1. 팀 구성원 및 업무 분장](#팀-구성원-및-업무-분장)

- [2. 와이어 프레임](#와이어-프레임)

- [3. DB 모델링](#DB-모델링)

- [4. 식도랑 시퀀스](#식도랑-시퀀스)

- [5. 핵심 기능](#핵심-기능)



## 팀 구성원 및 업무 분장

#### 정승희

 - 팀장 / QA / 프론트
     - 프로젝트 관리 전반 및 스케줄링
     - 지도 API 및 프론트
     - 이미지 처리 및 텍스트 추출 방문 알고리즘( OpenCV + Tesseract OCR )



#### 박인영

- 테크리더 / 프론트
  - 최종 코드리뷰 담당
  - 모바일 웹 최적화



#### 박도희

- 기획 / 프론트
  - 프로젝트 동영상 편집
  - 


#### 조규성

- 풀스택
  - 형태소 분석
  - 디버깅



#### 허성수

- 백엔드 / 배포
  - DB 모델링 설계 및 API 로직 작성
  - EC2, Jenkins, Nginx, uwsgi 를 통한 배포



## 와이어 프레임

- [식도랑_와이어프레임.pdf](https://github.com/Jokyuseong/Sikdorang/blob/main/%EC%82%B0%EC%B6%9C%EB%AC%BC/%EC%82%B0%EC%B6%9C%EB%AC%BC_%EC%8B%9D%EB%8F%84%EB%9E%91_%EC%99%80%EC%9D%B4%EC%96%B4%ED%94%84%EB%A0%88%EC%9E%84.pdf) 

- [식도랑_와이어프레임2.pdf](https://github.com/Jokyuseong/Sikdorang/blob/main/%EC%82%B0%EC%B6%9C%EB%AC%BC/%EC%82%B0%EC%B6%9C%EB%AC%BC_%EC%8B%9D%EB%8F%84%EB%9E%91_%EC%99%80%EC%9D%B4%EC%96%B4%ED%94%84%EB%A0%88%EC%9E%842.pdf) 

- [식도랑 와이어프레임3.pdf](https://github.com/Jokyuseong/Sikdorang/blob/main/%EC%82%B0%EC%B6%9C%EB%AC%BC/%EC%82%B0%EC%B6%9C%EB%AC%BC_%EC%8B%9D%EB%8F%84%EB%9E%91_%EC%99%80%EC%9D%B4%EC%96%B4%ED%94%84%EB%A0%88%EC%9E%843.pdf)



## DB 모델링

![ERD](README_img/ERD.PNG)





## 식도랑 시퀀스

- [식도랑_시퀀스.md](https://github.com/Jokyuseong/Sikdorang/blob/main/%EC%82%B0%EC%B6%9C%EB%AC%BC/%EC%82%B0%EC%B6%9C%EB%AC%BC_%EC%8B%9D%EB%8F%84%EB%9E%91_%EC%8B%9C%ED%80%80%EC%8A%A4.md)





## 핵심 기능

> **사용자와 연결된 태그, 카테고리를 필터링하여 음식점, 카페, 숙박, 관광지와 같은 여행 일정 추천 알고리즘 제공**
>
> 다이닝코드 식당 데이터, 한국관광공사 API를 사용하여 약 5만건의 데이터를 필터링
>
> 이상형 월드컵을 통해 초기 데이터 확보 및 코사인 유사도 분석으로 콜드스타트 문제 해결
>
> 카카오 map API를 사용하여 사용자가 고르거나 식도랑에서 추천받은 지점 자동으로 연결 및 거리 분석
>
> 리뷰를 쓰면 형태소 분석을 통해 리뷰에 사용한 글자 기반으로 사용자 태그 업데이트 구현
>
> IAMPORT API를 사용하여 이니시스, 카카오, 네이버페이 등 다양한 결제 시스템 구축
>
> Pytesserect, Open CV를 통해 영수증, 결제내역 분석으로 자동 방문 인증 구현



#### 구현기능

휴대폰 인증을 통한 가이드 권한 획득

사용자 여행 생성 후 동행구하기 활성화 가능

가이드일 경우 투어 생성을 통해 결제시스템 사용 가능

GeoLocation API를 통해 현재 위치 획득



---
