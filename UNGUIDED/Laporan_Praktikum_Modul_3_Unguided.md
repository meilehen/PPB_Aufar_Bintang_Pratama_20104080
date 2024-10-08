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
**Aisyah Hasna Aulia**  
**Muhammad Faza Zulian**

Dosen Pengampu :  
**Yudha Islami Sulistya, S.Kom., M.Cs**

**PROGRAM STUDI S1 REKAYASA PERANGKAT LUNAK  
FAKULTAS INFORMATIKA  
TELKOM UNIVERSITY PURWOKERTO  
2024**

</div>

# UNGUIDED

## Looping
```dart
import 'dart:io';

void main(List<String> args) {
  stdout.write('Input jumlah baris piramid: ');
  int baris = int.parse(stdin.readLineSync()!);

  for (var i = 1; i <= baris; i++) {
    for (var j = i; j < baris; i++) {
      stdout.write(' ');
    }

    for (var k = 1; k <= (2 * i - 1); i++) {
      stdout.write('*');
    }

    print('');
  }
}
```

---

## Function
```dart
import 'dart:io';

void main(List<String> args) {
  print('Input Bilangan Bulat: ');
  int? bilangan = int.parse(stdin.readLineSync()!);

  if (prima(bilangan)) {
    print('$bilangan ini adalah bilangan prima');
  } else {
    print('$bilangan ini bukan bilangan prima');
  }
}

bool prima(int bilangan) {
  if (bilangan <= 1 ) {
    return false;
  }

  for (int i = 2; i <= bilangan ~/ 2; i++) {
    if (bilangan % i == 0) {
      return false;
    }
  }

  return true;
}
```

---

## Branching
```dart
import 'dart:io';

void main() {
  print('Masukkan Nilai: ');
  int? nilai = int.parse(stdin.readLineSync()!);

  String hasil = periksaNilai(nilai);
  if (hasil.isNotEmpty) {
    print('$nilai merupakan $hasil');
  } else {
    print('90');
  }
}

String periksaNilai(int nilai) {
  if (nilai > 70) {
    return 'Nilai A';
  } else if (nilai > 40 && nilai <=70) {
    return 'Nilai B';
  } else if (nilai > 0 && nilai <= 40) {
    return 'Nilai C';
  } else {
    return '';
  }
}
```

---
