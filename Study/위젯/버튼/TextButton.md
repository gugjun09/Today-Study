# TextButton

글자만 표시되는 버튼 

**기본**

```
TextButton(
          child: Text('Text Button', style: TextStyle(color: Colors.red)),
          onPressed: () {
            print('Text 버튼 클릭!');
          },
        )
```

**두께 바꾸기**

```
TextButton(
          child: Text(
            'Text Button',
            style: TextStyle(fontWeight: FontWeight(500)),
          ),
          onPressed: () {
            print('Text 버튼 클릭!');
          },
        )
```
