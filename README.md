Study
====
Post what I have studied.
___
Algorithm
----
- 백준 10809번 FindAlphabet

- 백준 2675번 RepeatingCharacters

- 백준 1152번 단어의 개수
  > 문장 맨 앞, 뒤에도 공백이 들어갈 수 있다. 따라서 공백만 입력될 수도 있다.
공백만 입력됬을 때도 array.length가 1이 나오므로 그 점을 유의해야된다.

- 백준 1157번 단어 공부
  > Scanner를 close() 해주지 않아 런타임오류가 발생했었다.

- 백준 2908번 상수
  > StringBuffer를 이용해서 문자열을 거꾸로 바꿨다.

- 백준 5622번 다이얼

- 백준 1316번 그룹 문자 체커

- 백준 2941번 크로아티아 알파벳
  > substring()을 사용할 때 String의 index를 넘어가서 런타임 오류가 발생했다. if(String.length()>1)로 변경해서 해결했다.

- 백준 1712번 손익분기점

- 백준 2839번 설탕 배달
  > recursive하게 하니 시간 제한에 걸려서 실패했다. 반복으로 다시 짜서 해결했다.

- 백준 2292번 벌집
  > 원의 round가 같으면 도달하는 길이가 다 같은 문제였다.
  
- 백준 1193번 분수찾기

- 백준 10250번 ACM 호텔
  > 방번호가 한 자리 수 일때만 사이에 0이 들어가지만 두 자리 수 일때는 0이 들어가지 않는 데 0을 출력해서 틀렸었다. String.format을 이용해서 총 두 자리 중 빈자리는 0으로 채우게 했다.

- 백준 2869번 달팽이는 올라가고 싶다

- 백준 2775번 부녀회장이 될테야

- 백준 1011번 Fly me to the Alpha Centauri
  > 규칙을 찾지못해서 백준의 게시판에서 관련 팁을 봤지만 그래도 이해하지 못했다. 인터넷에 찾아보니 표를 그려서 전체적으로 보고 규칙을 찾아 간단하게 문제를 푸는 것을 발견했다. 그 글을 통해 풀었다. 출처: https://st-lab.tistory.com/79
  
- 백준 1978번 소수 찾기
  > 2일 때 소수가 아닌 수로 되어서 틀렸다. if 문으로 2를 따로 처리해줬다.
  
- 백준 2581번 소수
  > 2일 때 소수가 아닌 수로 되어서 오류가 났었다. if 문으로 2를 따로 처리해줬다.

- 백준 1929번 소수 구하기
  > 에라토스체네스의 체를 이용해서 푸는 문제였다.

- 백준 4948번 베르트랑 공준
  > 에라토스체네스의 체를 응용해서 풀었다.

- 백준 9020번 골드바흐의 추측
  > 배열의 index가 넘어간 범위를 접근해서 런타임 에러가 났다. index가 넘어간 원인은 에라토스테네스의 체 연산을 하는 과정에서 오류가 있었다. 해당 오류를 고치니 해결됬다.

- 백준 1085번 직사각형에서 탈출

- 백준 3009번 네번째 점

- 백준 4153번 직각삼각형

- 백준 3053 택시 기하학
  > 유클리드 기하학과 택시 기하학을 이용하는 문제였다.
  
- 백준 1002번 터렛
  > 두 원의 교점의 개수를 구하는 문제였다. 자바에서는 double형의 값을 비교할 때는 근사치로 비교해서 ex) 0.1+0.2=0.3 할 경우 같지 않다는 결과가 나온다고 한다. 그걸 몰라서 처음엔 계속 틀렸다. double형이 나오지 않도록 비교하는 값들은 제곱해서 int 형으로 비교하였다.
  
- 백준 10872번 팩토리얼

- 백준 10870번 피보나치 수 5

- 백준 2447번 별 찍기 - 10
  > char 배열에 하나하나 별을 넣고 StringBuilder로 합쳐서 출력했다.

- 백준 11729 하노이 탑 이동 순서

### 브루트 포스
- 백준 2231번 분해합

- 백준 2798번 블랙잭

- 백준 7568번 덩치

- 백준 1018번 체스판 다시 칠하기

- 백준 1436번 영화감독 숀

### 정렬
- 백준 2750번 수 정렬하기
  > 삽입 정렬을 사용했다.
  
- 백준 2751번 수 정렬하기 2
  > 합병 정렬을 사용했다.

- 백준 10908번 수 정렬하기 3
  > counting sort를 사용했다.
  
- 백준 2108번 통계학
  > 산술 평균을 구할 때 Math.round를 썼다. 그걸 썼을 때 음수는 값이 이상하게 나왔는 데 int / int는 int로 값이 나와서 그랬던 거였다. sum을 double형으로 바꿔주고 계산하니 제대로 반올림 된 값이 나왔다.
  
- 백준 1427번 소트인사이드

- 백준 11650번 좌표 정렬하기
  > Collections.sort()를 이용해서 정렬했다. Point에 compareTo를 구현하여 이용했다.
  
- 백준 11651번 좌표 정렬하기2

- 백준 1181번 단어 정렬
  > 중복 단어가 들어오면 한번만 출력되야 하는 것을 빼먹어서 틀렸다. 먼저 단어를 arraylist에 중복 검사해서 넣어준 다음 새로운 arraylist에 Strings 객체로 넣어주었다. Collections.sort()를 이용해서 정렬하기 위해 객체에 저장을 했다.
  
- 백준 10814번 나이순 정렬

### 백트래킹
- 백준 15649번 N과 M (1)
  > recursive 방식으로 풀었다. 0번째의 index부터 선택해주는 메소드를 만들어서 그 안에서 1번째 index 선택 메소드 호출 2번째 호출.. 이런 식으로 풀었다.
  
- 백준 15650번 N과 M (2)
  > 처음에 넣었던 조건이 index가 0일 경우는 아예 탐색을 안하게 하는 조건이여서 틀렸다. 조건을 바꿔 index와 arr[index-1]의 수에 따라 i의 초기값을 변경해주는 걸로 풀었다.
  
- 백준 15651번 N과 M(3)
  > 중복 수가 되기 때문에 출력하는 양이 많아서 시간초과가 났다. BufferedWriter를 이용하여 출력 시간을 줄여 통과했다.

- 백준 15652번 N과 M(4)

- 백준 9663번 N-Queen
  > 대각선의 queen을 확인하는 방법을 고민했는 데 찾아보니 두 행의 차와 두 열의 차 값이 같으면 서로 대각선에 존재하여서 그 방법을 이용해 풀었다.

- 백준 14888번 연산자 끼워넣기

- 백준 14889번 스타트와 링

### 동적계획법 1
- 백준 2748번 피보나치 수 2
  > 90번 째 피보나치 수는 int형의 범위를 넘어가서 틀렸다. long으로 바꿔주니 해결됐다.

- 백준 1003번 피보나치 함수

- 백준 1904번 01타일
  > mod 연산을 하고 값을 저장하는 것과 하지 않고 저장하는 것의 값이 달랐다. 이유는 더하다보면 값이 int의 범위를 초과하기 때문이였다. 따라서 마지막에 값을 다 구하고 mod 연산을 하지 않고 중간에 새로운 값을 저장할 때마다 mod 연산을 하였다. 또한 n의 값이 0, 1일 경우를 생각하여 tile[0], tile[1], tile[2]의 값을 저장하는 것에 if 문을 주었다.
 
- 백준 9461번 파도반 수열
  > 간단하게 수열의 규칙만 찾으면 쉬운 문제였다.
  
- 백준 1149번 RGB거리
  > 빨간색을 선택할 경우, 초록색을 선택할 경우, 파랑색을 선택할 경우를 다 구한 후 최소값을 출력하는 문제였다. 그 과정에서 직전 값을 비교하여 더 작은 값을 선택하는 부분이 있는 데 배열이 아닌 int로 저장했기 때문에 그걸 진행하고 나면 값이 바뀌기 때문에 그 이후에 영향을 미쳐서 문제가 발생했다. 직전 값을 따로 다 저장하고 비교했다.
  
- 백준 1932번 정수 삼각형

- 백준 2579번 계단 오르기

- 백준 1463번 1로 만들기
  > 어떻게 풀지 생각이 안나서 다른 사람 코드를 확인했다. 처음엔 BFS로 풀어야되나 했는데 그냥 n 전까지의 숫자들이 1이 될려면 필요한 연산의 개수를 구해서 n/3, n/2, n-1등 n일 때 가능한 연산 중 가장 연산 수가 작은 걸 골라서 구하면 되는 문제였다.

- 백준 10844번 쉬운 계단 수
  > 결과 값을 구하는 방법은 알았지만 그 값을 구하는 수식이 있는 줄 알았는 데 아니였다. 이중 배열을 써도 되는 데 굳이 계속 일차원 배열을 쓸려고 고집하다보니 혼자서 풀지 못했다. 그래도 저번보단 좀 더 문제에서 구해야되는 것(계단 수)에 집중해서 접근했다.
  
- 백준 2156번 포도주 시식
  > 2579번 계단 오르기에서 약간 변형된 문제라서 그걸 수정해서 풀면 될 줄 알았는 데 풀리지 않았다. 다른 사람들의 답을 찾아보니 계단 오르기도 내가 좀 복잡하게 생각해서 푼 거였다. 계단을 연속해서 밟을 경우와 안 밟을 경우를 다 저장해서 풀었는 데, 그냥 xoo, oxo인 경우를 구해서 둘 중 더 큰 값만 저장하면 되는 거 였다. 이걸로 다시 수정해서 풀어서 지금의 답이 나왔다. xoo, oxo, oox인 3가지 경우를 비교하여 더 큰 값을 저장하였다.
___
- 프로그래머스 크레인 인형 뽑기 게임
  > 크레인이 뽑는 위치는 column인데 row로 생각해서 틀렸다. column으로 바꾸니 맞았다.
_______
Data Structure
--
- 스택 자바 구현
- 선형 큐 자바 구현
- 원형 큐 자바 
