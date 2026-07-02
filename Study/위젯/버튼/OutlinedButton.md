# OutlinedButton 

테두리만 있는 버튼 위젯

기본
```dart
OutlinedButton(     
  onPressed: () {
    print('Outlined 버튼 클릭!');
  },
  child: Text('Outlined Button'),
)
```

색 바꾸기

```dart
OutlinedButton(
  style: OutlinedButton.styleFrom(
    backgroundColor: Colors.yellow,
    side: BorderSide(color: Colors.red) // 테두리 변경
  ),
  ...
)
```
