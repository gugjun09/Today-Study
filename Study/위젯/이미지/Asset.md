# Asset 이미지

**앱 내 로컬 파일을 사용한다.**

등록하는법:


[pubspec.yaml]

```
flutter:
  assets:
    - assets/images/
```

예시 : 

```
Image.asset(
  'assets/images/example.png',
  width: 100,
  height: 100,
  fit: BoxFit.cover, // 위젯 크기에 맞추어 이미지 꽉 채운다.
)
```

