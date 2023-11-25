# omok_game
오목 게임 미션



### 개요

19 x 19 바둑판에 돌을 놓아 오목을 판별하는 함수를 만듭니다.

아래의 함수 명세에 맞춰 check_omok() 함수를 구현합니다.



### [함수 명세]

- check_omok 함수는 board, x, y, dol 전달인자를 받아 오목을 판별하여 문자열 결과를 반환합니다.

- board는 19 x 19 크기의 이차원 배열입니다. 아래와 같이 바둑판 위에 놓여진 돌을 표현합니다.

   '.' -> 돌이 놓이지 않음

   'o' -> 백돌이 놓임

   'x' -> 흑돌이 놓임

- 함수에 전달되는 board는 오목 게임에서 유효한 입력 상태를 갖는다고 가정합니다.

- x는 가로축 위치, y는 세로축 위치를 의미합니다.

- dol은 board에 새로 놓일 돌을 의미합니다. 'o'와 'x'만 입력된다고 가정합니다.



###  [함수 반환 값]

check_omok 함수가 다음 케이스에 맞춰 값을 반환할 수 있도록 구현합니다. 

각각의 구현 여부에 따라 부분 점수를 부여합니다.



- "INVALID_BOARD_SIZE": board의 크기가 19 x 19 가 아닌 경우 반환

- "INVALID_POSITION": x와 y가 0~18 사이가 아 니거나 이미 돌이 놓여져있는 경우

- "VICTORY_WHITE": 백돌이 오목을 완성한 경우 / 흑돌이 육목이 완성된 경우

- "VICTORY_ BLACK": 흑돌이 오목을 완성한 경우 / 백돌이 육목이 완성된 경우

- "CONTINUE_GAME": dol이 놓여져도 게임이 종료되지 않는 경우



### [평가 기준]

테스트 코드를 참고하여 최상단의 check_omok 함수를 완성하시면 됩니다.

각 케이스의 테스트 코드가 PASS될 때 아래와 같은 부분 점수를 받게됩니다.


- 총 20점
- INVALID_BOARD_SIZE case 만족 : 5점
- INVALID_POSITION case 만족: 6점
- VICTORY_WHITE, VICTORY_BLACK case 만족: 5점
- VICTORY_WHITE, VICTORY_BLACK sixmok case 만족: 2점
- CONTINUE_GAME case 만족 및 문제 의도에 맞게 적절하게 구현했다면: 2점
