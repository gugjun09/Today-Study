# AnimatedSlide

AnimatedSlide 는 지정된 위치가 변경될 때마다 지정된 시간 동안 자식 요소의 위치를 ​​자동으로 전환한다.


```

class Sk extends StatefulWidget {
  const Sk({super.key});

  @override
  State<Sk> createState() => _SkState();
}

class _SkState extends State<Sk> {
  Offset start = Offset(3, 2);  // 처음 위치

  @override
  void initState() {
    super.initState();

    Future.delayed(Duration(seconds: 3), () {   //  실행한 후 움직일 때까지 대기시간
      setState(() {
        start = Offset(0, 5);  // 이동할 위치
      });
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Stack(
        children: [
          AnimatedSlide(
            offset: start,
            duration: Duration(seconds: 2),  // 애니메이션 동적 시간
            curve: Curves.elasticOut,  // 애니메이션 스타일

            child: Container(width: 100, height: 100, color: Colors.blue),
          ),
        ],
      ),
    );
  }
}

```
