# pjt 02 Python을 활용한 데이터 수집 II



## 1. 개발 환경


- **A. 언어**

  - python 3.8 이상

- **B. 도구**


    - vsCode

- **C. 필수 라이브러리**


    - json
    - requests

## 2. 요구사항

커뮤니티 서비스 개발을 위한 데이터 수집 단계로, 전체 데이터 중 필요한 데이터를 크롤링 하는 과정을 진행합니다. 아래 기술된 사항은 필수적으로 구현해야 하는 내용입니다.

---

#### A. 영화 개수 카운트 기능 구현

영화 개수를 출력합니다. 완성된 기능은 향후 커뮤니티 서비스에서 제공되는 기능으로 사용됩니다.

---

#### B. 특정 조건에 맞는 영화 출력

popular를 기준으로 가져온 영화 목록 중 평점이 8 이상인 영화 목록을 출력하는 기능을 완성합니다.

---

#### C. 평점 순 정렬

popular를 기준으로 가져온 영화 목록을 평점순으로 출력하는 함수를 완성합니다. 해당 기능은 향후 커뮤니티 서비스에서 기본으로 제공되는 영화 정보로 사용됩니다.

---

#### D. 제목 검색, 영화 추천

해당영화를 기준으로 추천영화 목록을 출력하는 함수를 완성합니다. 해당 기능은 향후 커뮤니티 서비스에서 추천영화 기능으로 사용됩니다.

---

#### E. 배우, 감독 리스트 출력

영화에 출연한 배우들과 감독의 정보가 저장된 딕셔너리를 출력하는 함수를 완 성합니다. 해당 기능은 향후 커뮤니티 서비스에서 기본으로 제공되는 영화 정보로 사용됩니다.

---



## 3. 프로세스

#### A. 영화 개수 카운트 기능 구현

1. 인스턴스 생성

2. 영화 리스트를 조회할 URL 생성
3. requests 패키지를 이용하여 URL에 요청
4. 영화 리스트의 정보 개수 반환



#### B. 특정 조건에 맞는 영화 출력

1. 인스턴스 생성

2. 영화 리스트를 조회할 URL 생성
3. requests 패키지를 이용하여 URL에 요청
4. 평점이 8 이상인 영화 목록 반환



#### C. 평점 순 정렬

1. 인스턴스 생성

2. 영화 리스트를 조회할 URL 생성
3. requests 패키지를 이용하여 URL에 요청
4. 영화 정보 리스트 생성
5. vote_average을 기준으로 내림차순 정렬 후 반환



#### D. 제목 검색, 영화 추천

1. 인스턴스 생성

2. 영화 제목에 대한 id 변환
3. movie id가 있으면, 영화 추천 URL 생성 후 영화 제목 리스트 생성
4. movie id가 없으면 None 반환

#### E. 배우, 감독 리스트 출력

1. 인스턴스 생성

2. 영화 제목에 대한 id 변환
3. movie id가 있으면, 영화 credits URL 생성 후 배우, 감독 리스트 생성
4. movie id가 없으면 None 반환



## 4. 느낌점

API를 직접 사용해보면서, 데이터를 직접 수집하여 원하는 데이터로 반환하는 것에 대해 새로움을 느꼈다. 또한, 서버에 요청을 보내 정보를 얻은 경험이 얼마 없었기에, 이번 프로젝트는 더욱 기억에 남을 것 같다.