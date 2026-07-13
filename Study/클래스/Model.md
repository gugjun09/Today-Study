## Model

Model은 앱이 다루는 데이터의 구조와 상태를 정의하고 관리하는 핵심 오쇼이다. 

내가 배우고 있는 모델은 상태 모델이다(State/App Model)

상태 모델은 데이터를 추가, 삭제, 수정하는 로직을 포함하며, 데이터가 변경되면 화면에 이를 알린다.

```

class UserModel {
  final int id;
  String name;
  final int r;
  final int g;
  final int b;

  UserModel({
    required this.id,
    required this.name,
    required this.r,
    required this.g,
    required this.b,
  });

  factory UserModel.createUserModel() {
    return UserModel(
      id: DateTime.now().millisecondsSinceEpoch,
      name: '',
      r: Random().nextInt(256),
      g: Random().nextInt(256),
      b: Random().nextInt(256),
    );
  }

  factory UserModel.fromJson(Map<String, dynamic> json) {
    return UserModel(
      id: json['id'],
      name: json['name'],
      r: json['r'],
      g: json['g'],
      b: json['b'],
    );
  }

  Map<String, dynamic> toJson() {
    return {'id': id, 'name': name, 'r': r, 'g': g, 'b': b};
  }
}

```
