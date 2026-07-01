# length

문자열의 길이 출력용 함수.

반환 값이 Int라서 Text 같은 곳에서 사용할 땐 String 으로 변환 해줘야 함.

```
'Dart'.length;          // 4
'Dart'.runes.length;    // 4
var clef = '\\u{1D11E}';
clef.length;            // 2
clef.runes.length;      // 1
```
