# StatelessWidget

한번 그려진 후에는 변경되지 않는 위젯이다. 예를 들어, 앱의 로고 이미지나 정적인 텍스트를 표시하는 데 사용된다.

화면이 로드될 때 한 번만 그려지는 State가 없는 위젯으로 변겨이 필요한 Data가 없는 것을 의미하며 이벤트 또는 사용자 상호 작용에 의해 동작하지 않는다.

```

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        
        child: Icon(Icons.search,size: 100,),
      ),
    );
  }
}
```


# Stateful Widget 

위젯이 동작하는 동안 Data 변경이 필요한 경우 화면을 다시 그려서 변경된 부분을 위젯에 반영하는 동적인 위젯으로 이벤트 또는 사용자 상호 작용에 의해 동작한다.  

예를 들어 축구 게임의 경우 점수를 나타내는 위젯은 골이 들어갈 때마다 변경해야 돼서 Stateful Widget 사용이 필요하다.

```

class HomeScreen extends StatefulWidget {
  const HomeScreen({super.key});

  @override
  State<HomeScreen> createState() => _HomeScreenState();
}

class _HomeScreenState extends State<HomeScreen> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        child: CupertinoDatePicker(mode: CupertinoDatePickerMode.date,
          onDateTimeChanged: (DateTime date) {

          },
          dateOrder: DatePickerDateOrder.ydm,

        ),
      ),
    );
  }
}
```

**빌드 과정을 기준으로 두 위젯을 비교하면 다음과 같다.**

Stateless Widget은 한 번만 Build 과정이 발생하여 한번 그려진 화면은 계속 유지되며, 성능이 좋다. 

Stateful Widget은 setState가 발생 시 다시 Build 하는 과정이 일어나며 동적 화면을 구현할 수 있다.
