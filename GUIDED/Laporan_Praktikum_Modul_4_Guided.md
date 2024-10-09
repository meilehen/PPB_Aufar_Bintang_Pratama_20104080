<div align="center">

**LAPORAN PRAKTIKUM**  
**PEMROGRAMAN PERANGKAT BERGERAK**

**MODUL 4**  
**USER INTERFACE**

![logo tel-u](https://github.com/user-attachments/assets/3a44181d-9c92-47f6-8cf0-87755117fd99)

Disusun Oleh :

**Aufar Bintang Pratama (20104080)**  
**SE04-03**

Asisten Praktikum :  
**Aisyah Hasna Aulia**  
**Muhammad Faza Zulian**

Dosen Pengampu :  
**Yudha Islami Sulistya, S.Kom., M.Cs**

**PROGRAM STUDI S1 REKAYASA PERANGKAT LUNAK  
FAKULTAS INFORMATIKA  
TELKOM UNIVERSITY PURWOKERTO  
2024**

</div>

# GUIDED

## A. Grid View
**Input**
```dart
import 'package:flutter/material.dart';

class gridView extends StatefulWidget {
  const gridView({super.key});

  @override
  State<gridView> createState() => _MyHomePageState();
}

class _MyHomePageState extends State<gridView> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Praktikum Modul 4'),
        backgroundColor: Colors.blue,
      ),
      body: GridView.count(
        crossAxisCount: 4,
        mainAxisSpacing: 10,
        crossAxisSpacing: 10,
        padding: EdgeInsets.all(12),
        children: [
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 0'),
            color: Colors.yellow,
          ),
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 1'),
            color: Colors.blue,
          ),
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 2'),
            color: Colors.red,
          ),
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 3'),
            color: Colors.green,
          ),
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 4'),
            color: Colors.purple,
          ),
          Container(
            padding: EdgeInsets.all(10),
            child: Text('Grid View 5'),
            color: Colors.brown,
          ),
        ],
      ),
    );
  }
}
```
**Output**

![image](https://github.com/user-attachments/assets/96e23fcb-7f2a-441c-a8cc-06981d79351e)


---

### B. List View
**Input**
```dart
import 'package:flutter/material.dart';

class Listview extends StatelessWidget {
  const Listview({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(title: Text('Latihan List View '),
      backgroundColor: Colors.amber,
      ),
      body: ListView(
        scrollDirection: Axis.horizontal,
        children: [
          Container(
            height: 200,
            width: 200,
            color: Colors.red,
            child: Center(child: Text('Type A'),),
          ),
          Container(
            height: 200,
            width: 200,
            color: Colors.yellow,
            child: Center(child: Text('Type B'),),
          ),
          Container(
            height: 200,
            width: 200,
            color: Colors.green,
            child: Center(child: Text('Type C'),),
          ),
        ],
      ),
    );
  }
}
```

![image](https://github.com/user-attachments/assets/8962e447-113d-42aa-a571-14678afaefbf)


---
## C. Stack
**Input**
```dart
import 'package:flutter/material.dart';

class stackScreen extends StatelessWidget {
  const stackScreen({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Latihan Stack'),
        centerTitle: true,
        backgroundColor: Colors.blue,
      ),
      body: Stack(
        children: [
          Container(
            margin: EdgeInsets.all(8),
            width: 100,
            height: 100,
            color: Colors.red,
          ),
          Container(
            margin: EdgeInsets.all(4),
            width: 100,
            height: 100,
            color: Colors.green,
          ),
          Container(
            margin: EdgeInsets.all(2),
            width: 100,
            height: 100,
            color: Colors.blue,
          ),
        ],
      ),
    );
  }
}
```
**Output**

![image](https://github.com/user-attachments/assets/24e99159-3727-4748-9fad-65183c84059d)
