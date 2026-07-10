# Stack

위젯의 자식 요소들을 부모위의 가장자리를 기준으로 배치하는 위젯이다.

```
Stack(
children: [
  Container(
   width: 100,
     height: 100,
   color: Colors.red,
  ),
  Container(
   width: 90,
   height: 90,
   color: Colors.green,
   ),
   Container(
    width: 80,
   height: 80,
     color: Colors.blue,
            ),
          ],
        ),
```

 텍스트와 이미지를 겹쳐 놓고 하단에 버튼을 추가하는 등 여러 자식 요소를 간단하게 겹쳐 표시하고 싶을 때 유용하다.
