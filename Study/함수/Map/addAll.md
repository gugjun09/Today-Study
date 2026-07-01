#addAll

Map의 key/value 값을 추가하는 함수이다.

```
final planets = <int, String>{1: 'Mercury', 2: 'Earth'};
planets.addAll({5: 'Jupiter', 6: 'Saturn'});
print(planets); // {1: Mercury, 2: Earth, 5: Jupiter, 6: Saturn}
```
만약 추가하고싶은 key/value값이 Map에 이미 있다면 그 값은 덮여진다. 
