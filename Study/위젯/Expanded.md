# Expanded

Row, Column 또는 Flex의 자식을 확장하여 자식이 사용 가능한 공간을 채우는 위젯이다.

Expanded 위젯을 사용하면 Row, Column, Flex 의 자식 위젯이 주축을 따라 사용 가능한 공간을 채우도록 확장된다.


```
Row(
        children: [
          Container(color: Colors.yellow,  width: 100, height: 100,),
          Expanded(child: Container(color: Colors.blue,  height: 100,)),  // 채울 수 있는 공간 모두 확장

          Container(color: Colors.red,  width: 100,height:  100),
        ],
      ),
```

Expanded는 공간에 차지하는 데에 있어서 중요한 위젯 중 하나이다.

Flex로 공간차지 비율을 정할 수 있다.
