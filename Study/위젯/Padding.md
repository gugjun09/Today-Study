# Padding

지정된 패딩만큼 자식 위젯을 안쪽으로 밀어 넣는 위젯.

```
Padding(
  padding: EdgeInsets.all(16.0),
  child: Text('Hello World!'),
),
```

패딩의 프로퍼티인 `padding`은  `EdgeInsetsGeometry` 타입인데 굳이 이 위젯 사용 안하고 `EdgeInsets` 사용해주면 됨.

---

`EdgeInsets` 에는 생성 4개가 있음.

- `EdgeInsets.all` -> 모든 부분에 패딩을 먹여줌
```
EdgeInsets.all(8.0)
```

- `EdgeInsets.symmetric` -> 가로/세로를 지정해서 패딩을 먹일 수 있음
```
EdgeInsets.symmetric(vertical: 8.0) // 세로 패딩
EdgeInsets.symmetric(horizontal: 8.0) // 가로 패딩
```
