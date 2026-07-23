# ListView.builder

많은 양의 데이터를 터치해서 스크롤 가능한 목록으로 만들 때 사용하는 위젯이다.

일반 Listview는 모든 데이터를 한 번에 메모리에 올리기 때문에 데이터가 많을 경우 성능이 저하된다. 
그러나 ListView.builder는 현재 화면에 보이는 거나 그 주변의 있는 것만 생성하므로 대용량 리스트에 적합하다.



```

class Sk extends StatefulWidget {
  const Sk({super.key});


  @override
  State<Sk> createState() => _SkState();
}

final List<String> items = List.generate(20, (index) => '항목',);   

class _SkState extends State<Sk> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: ListView.builder(
        itemCount: items.length,  // 리스트의 항목 갯수

        itemBuilder: (context, index) {
          return ListTile(
            leading: FlutterLogo(),  // 리스트 왼쪽 요소
            title: Text(items[index]), // 리스트 타이틀

            trailing: Icon(Icons.search),  // 리스트 오른쪽 요소
          );
        },
      ),
    );
  }
}

```
