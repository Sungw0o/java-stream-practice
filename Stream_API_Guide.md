# Stream API

## 복잡한 함수나 알고리즘을 함수형 프로그래밍 기법을 사용해 간결하게 처리해줌

### 주요 특징
- 비순차 처리 : 데이터를 병렬로 처리 할 수 있는 기능 제공
- 내부 반복 : 외부 반복(Ex.for) 대신 내부 반복을 사용해 복잡성을 줄이고, 가독성을 향상
- 연산 체이닝 : 여러 연산을 체인처럼 연결해 복잡한 데이터를 처리 가능

## 생성 -> 가공 -> 처리 순으로  이루어진다.

### 생성
- 순차/병렬 스트림
- 기본 타입/String/File 스트림
- Stream.builder()/ Stream.generate()/ Stream.iterate()/ Stream.of()-> 스트림 클래스로 객체 생성

### 가공
- Filtering : 조건에 맞는 원소 추출
- Mapping : 객체의 각 원소들에 대해 결과와 매칭시킴
- Sorting : 순서에 맞게 원소를 정렬
- Iterating : 원소를 읽어들임

### 처리
- Calculating : map : 스트림 각 요소에 함수 적용 결과를 새로운 스트림으로 반환
- Reducing : reduce : 스트림의 각 요소들을 하나의 요약된 결과로 축소(합계, 최댓값)
- Collecting: collect : 스트림의 결과를 다양한 형태의 컬렉션을 수집(List,Set,Map 변환)
- Matching : any,all,noneMatch : 스트림 요소들이 조건에 부합하는지 검사(하나라도 일치, 모두 일치, 일치하지 않는 요소 순)
- Iterating : forEach : 스트림 각 요소에 대한 주어진 반복 작업을 수행