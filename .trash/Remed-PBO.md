void main() {
  // List bahan
  List<String> bahanBaru = ['Serat Karbon', 'Keramik', 'Asbes', 'Logam'];

  // Operator
  bool containsAsbes = bahanBaru.contains('Asbes');
  print('Mengandung Asbes: $containsAsbes');

  // Map
  Map<String, double> bahanHarga = {
    'Serat Karbon': 200.0,
    'Keramik': 150.0,
    'Asbes': 100.0,
    'Logam': 50.0
  };

  // Percabangan
  bahanBaru.forEach((bahan) {
    if (bahanHarga[bahan]! > 50) {
      print('$bahan mahal.');
    } else {
      print('$bahan murah.');
    }
  });

  // Set
  Set<String> bahanUnik = bahanBaru.toSet();
  print('Bahan unik: $bahanUnik');

  // Function dengan parameter dan optional parameter
  void printHargaBahan(String bahan, {double discount = 0}) {
    double harga = bahanHarga[bahan] ?? 0;
    double finalHarga = harga - (harga * discount);
    print('Harga $bahan dengan diskon ${discount * 100}%: $finalHarga');
  }

  printHargaBahan('Serat Karbon', discount: 0.1);
  printHargaBahan('Logam');

  // Inner function dan anonymous function
  void prosesBahan(Function(String) action) {
    bahanBaru.forEach(action);
  }

  prosesBahan((bahan) {
    print('Proses bahan: $bahan');
  });

  // Closure
  Function tambahBahan(String bahan) {
    bahanBaru.add(bahan);
    return () {
      print('Bahan $bahan ditambahkan ke list.');
    };
  }

  var closure = tambahBahan('Kaca');
  closure();

  // Perulangan
  for (var bahan in bahanBaru) {
    print(bahan);
  }
}