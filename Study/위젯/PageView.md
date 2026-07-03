# PageView

여러 페이지(혹은 위젯)를 좌우 또는 상하로 스와이프하여 전환할 수 있게 해주는 스크롤 가능한 위젯이다.

```
PageView(
        children: [1, 2, 3, 4, 5] // 데이터 리스트
            .map((e) => Image.asset('asset/img/img_$e.png', fit: BoxFit.cover)) // 위젯으로 변환
            .toList(), // List<Widget> 형태로 변환
      ),
```


