# GestureDetector

클릭하면 특정 다트파일로 이동하는 위젯이다.

```
GestureDetector(
              onTap: () {
                Navigator.of(context).push(MaterialPageRoute(builder: (context) {
                  return AddProfileScreen(); 이동할 다트파일
                },));
              },
              child: Column(
                spacing: 6,
                children: [
                  Icon(Icons.add_circle_outline, size: 56, color: Colors.white), // 아이콘
                  Text('프로필 추가', style: TextStyle(color: Colors.white,
              
                  fontSize: 16)),
                ],
              ),
            ),
```
