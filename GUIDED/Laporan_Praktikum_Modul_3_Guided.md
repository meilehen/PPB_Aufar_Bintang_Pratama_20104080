<div align="center">

**LAPORAN PRAKTIKUM**  
**PEMROGRAMAN PERANGKAT BERGERAK**

**MODUL 3**  
**PENGENALAN DART**

![logo tel-u](https://github.com/user-attachments/assets/3a44181d-9c92-47f6-8cf0-87755117fd99)

Disusun Oleh :

**Aufar Bintang Pratama (20104080)**  
**SE04-03**

Asisten Praktikum :  
Aisyah Hasna Aulia  
Muhammad Faza Zulian

Dosen Pengampu :  
Yudha Islami Sulistya, S.Kom., M.Cs

PROGRAM STUDI S1 REKAYASA PERANGKAT LUNAK  
FAKULTAS INFORMATIKA  
TELKOM UNIVERSITY PURWOKERTO  
2024

</div>

# GUIDED

## A. Variabel
**Input**
```dart
void main() {
  String firstName = 'Praktikum';
  var lastName = 'PPB';
  final cuaca = 'Cerah';

  print('Hari ini $firstName $lastName');
}
```

**Output**

![image](https://github.com/user-attachments/assets/64bb2a8e-a03b-49b2-b7bb-ba0ebf0153c8)


---

## B. Control Flow
**Input**
```dart
void main() {

  // if else

  var open = 8;
  var close = 17;
  var now = 20;

  if (now >= open && now <= close) {
    print("We're open");
  } else {
    print("Sorry, we're closed");
  }

  var shop = now > open ? 'Shop Open' : 'Shop Closed';
  print(shop);

  // switch case

  var nilai = 'b';

  switch (nilai) {
    case 'a':
      print('Nilai Sangat Bagus');
      break;
    case 'b':
      print('Nilai Bagus');
    case 'c':
      print('Nilai Cukup');
      break;
    default:
      print('Nilai Tidak Tersedia');
  }
  
}
```
**Output**

![image](https://github.com/user-attachments/assets/f3a71cce-da45-4909-8387-bdafb9f954e4)
![image](https://github.com/user-attachments/assets/f84787ce-b1b2-4694-987a-a7ff52d75eba)


---

## C. Loop
**Input**
```dart
void main () {
  for (int i = 0; i < 5; i++) {
    print(i);
  }

  int i = 1;
  while (i <= 5) {
    print('Angka: $i');
    i++;
  }
}
```

**Output**

![image](https://github.com/user-attachments/assets/c1e2a16f-fec0-4804-b1ae-5541fd7c39b6)


---

## D. List
**Input**
```dart
  void main() {

   List<int> fixedList = List.filled(3, 0);

  fixedList[0] = 10;
  fixedList[1] = 20;
  fixedList[2] = 30;

  print('Fixed Length List: $fixedList');

List<int> growableList = [];

  growableList.add(10);
  growableList.add(20);
  growableList.add(30);

  print(growableList);

  growableList.add(50);
  growableList.add(60);
  growableList.add(70);

  print(growableList);

  growableList.remove(20);
  
}
```

**Output**

![image](https://github.com/user-attachments/assets/35424e52-6b73-4881-8d33-2a3b19f0a021)
![image](https://github.com/user-attachments/assets/1c7803e3-9a2f-44c3-bd93-50bc3cd91856)

---

## F. Function
**Input**
```dart
  void cetakPesan(String pesan) {
  print(pesan); // Mencetak pesan
}

int perkalian(int a, int b) {
  return a * b; // Mengembalikan nilai perkalian
}

void main () {
  int hasil = perkalian(7, 10);
  print("Hasil perkalian: $hasil");

  cetakPesan("Kamu Pintar");
}
```

**Output**

![image](https://github.com/user-attachments/assets/858dda5c-7b99-4cea-bdf3-582e48a77c73)

