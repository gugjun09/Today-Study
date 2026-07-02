# OutlinedButton : 테두리만 있는 버튼 위젯

```
OutlinedButton(
  child: Text('Outlined Button'),
  style: OutlinedButton.styleFrom(
    primary: Colors.orange, // 글자색
    side: BorderSide(color: Colors.orange, width: 2), // 테두리 설정
  ),
  onPressed: () {
    print('Outlined 버튼 클릭!');
  },
)
```

