# brainfuck
A brainfuck interpreter written in python

## 명령어
- `+` : 테이프가 가리키는 숫자를 1 증가시킨다.
- `-` : 테이프가 가리키는 숫자를 1 감소시킨다.
- `>` : 테이프를 한 칸 오른쪽으로 옮긴다.
- `<` : 테이프를 한 칸 왼쪽으로 옮긴다.
- `.` : 테이프가 가리키는 숫자를 ASCII 문자로 해석해서 출력한다.
- `,` : 문자를 하나 읽어서 그 ASCII 값을 테이프가 가리키는 위치에 저장한다. 파일의 끝(EOF, End of File)에서의 동작은 구현체마다 차이가 있다.
- `[…]` : 유일한 루프문. 매번 현재 테이프가 가리키는 숫자(매 루프마다 바뀔 수 있다)가 0인지 아닌지 체크해서, 조건이 만족되면 계속 안에 들어 있는 코드를 실행한다. 당연히 0번 실행될 수도 있다.
  - `[` : 포인터가 가리키는 바이트의 값이 0이 되면 짝이 되는 `]`로 이동한다. 의사코드로는 `while(*ptr != 0) {...}`이다.
  - `]` : 포인터가 가리키는 바이트의 값이 0이 아니면 짝이 되는 `[`로 이동한다.

## ASCII 코드표
![image](https://user-images.githubusercontent.com/61646760/147531437-a7af09ec-60d9-440b-8042-fddcc07e57a6.png)

## 참고
- [Brainfuck visualizer](https://brainfuck-visualizer.herokuapp.com/)
- [Brainfuck text generator](https://copy.sh/brainfuck/text.html)
- [브레인퍽 - 나무위키](https://namu.wiki/w/%EB%B8%8C%EB%A0%88%EC%9D%B8%ED%8D%BD)
- [브레인퍽 | 메아리 풉;](https://pub.mearie.org/%EB%B8%8C%EB%A0%88%EC%9D%B8%ED%8D%BD)
