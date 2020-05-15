# 한국주소API (KoreaAddressAPI)
한국 주소 API, juso.go.kr의 주소데이터 기반으로 만든 한국주소 API입니다.

아래와 같은 다양한 형태의 주소를 깨끗한 주소로 만들어주는 API로, R 과 Python을 사용하여 개발되었습니다.

사용법은 [여기](아직링크없다)를 참고하세요

---
입력주소 예제 #1 도로명주소로 입력되어 있는 주소 예제입니다.

* 특정지역명이 여러가지로 작성된 주소 / 서울/ 서울시/ 서울특별시
* 주소 중간에 필요없는 문자나 특수문자가 추가되어 있음


- 서울 관악구 남현3길 78, 덕원빌딩 6층
- 서울특별시, 관악구 남현3길, 78 덕원빌딩 6층
- 서울시 관악구 남현3길 78 덕원빌딩 6층

출력주소 예제 #1

|시/도|군/구|도로명 주소|건물이름|호수/상세위치|
|---|---|---|---|---|
|서울|관악구|남현3길 78|덕원빌딩|6층|

---

입력주소 예제 #2 지번 주소로 입력되어 있는 주소 예제입니다.

* 특정지역명이 여러가지로 작성된 주소 / 서울/ 서울시/ 서울특별시
* 지번주소에 '번지'와 같은 필요 없는 글자가 포함되어 있음


- 서울 관악구 남현동 602-1 6층
- 서울시 관악구 남현동 602-1 6층
- 서울특별시 관악 남현동 602-1번지 6층
- 서울특별시 관악 남현동 602-1 6층

출력주소 예제 #2

|시/도|군/구|동/읍/면|지번/리|건물이름|호수/상세위치|
|---|---|---|---|---|---|
|서울|관악구|남현동|602-1|   |6층|

---

입력주소 예제 #3 동/읍/면과 도로명 주소가 함께 입력되어 있는 주소 예제입니다.

* 도로명주소와 함께, 동/읍/면이 함께 포함되어 있음


- 서울특별시 관악구 남현동 남현3길 78 6층

출력주소 예제 #3

***어케 하는게 좋을려나, 고민중***

---

한국주소API(KoreaAddressAPI)는 DAT스터디에서 개발하였습니다.
 https://skysign.github.io/DAT ← 여기 참고하세요

---

이 프로젝트에 사용된 모든 주소/도로명/건물/상세주소 등의 데이터는 http://www.juso.go.kr/ 에서 제공하는 데이터를 사용하였습니다.

---
