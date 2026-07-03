# PageView

여러 페이지(혹은 위젯)를 좌우 또는 상하로 스와이프하여 전환할 수 있게 해주는 스크롤 가능한 위젯이다.

```
PageView(
        controller: controller,
        children: [1, 2, 3, 4, 5] // 데이터 리스트
            .map((e) => Image.asset('asset/img/img_$e.png', fit: BoxFit.cover)) // 위으로 변환
            .toList(), // List<Widget> 형태로 변환
      )
```


**수직으로 스크롤하기**

```
PageView(
        controller: controller,
        scrollDirection: Axis.vertical,
        children: [1, 2, 3, 4, 5]
            .map((e) => Image.asset('asset/img/img_$e.png', fit: BoxFit.cover))
            .toList(),
      ),
```
 
**PageController를 사용하면 뷰에 표시되는 페이지를 제어할 수 있다.**








