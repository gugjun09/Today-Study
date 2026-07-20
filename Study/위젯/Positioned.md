# Positioned

Stack의 자식 요소의 위치를 제하는 위젯이다.

위치 지정 위젯은 반드시 Stack의 하위 요소여야 한다. 그 외 다른 곳에서 사용 해버리면 바로 오류가 나버린다. 

```
Center(
          child: Container(
            height: 200,
            width: 200,
            color: Colors.blue[50],
            child: Stack(
              children: [
                Positioned(
                  top: 70,  // 높이 중간
                  left: 0,  // 맨 왼쪽
                  child: FlutterLogo(
                    size: 50,
                  ),
                ),
              ],
            ),
          ),
        ),
```
