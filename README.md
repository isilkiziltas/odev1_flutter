void main() {
  List<int> liste = [1, 2, 3, 4, 5];

  // Soru 1: Liste Elemanlarını Toplama
  int toplam = listeElemanlariniTopla(liste);
  print("Toplam: $toplam");

  // Soru 2: Tek Sayıları Filtreleme
  List<int> tekSayilar = tekSayilariFiltrele(liste);
  print("Tek Sayılar: $tekSayilar");

  // Soru 3: Listeyi Ters Çevirme
  List<int> tersListe = listeyiTersCevir(liste);
  print("Ters Liste: $tersListe");
}

// Soru 1: Liste Elemanlarını Toplama
int listeElemanlariniTopla(List<int> liste) {
  return liste.reduce((a, b) => a + b);
}

// Soru 2: Tek Sayıları Filtreleme
List<int> tekSayilariFiltrele(List<int> liste) {
  return liste.where((sayi) => sayi % 2 != 0).toList();
}

// Soru 3: Listeyi Ters Çevirme
List<T> listeyiTersCevir<T>(List<T> liste) {
  return liste.reversed.toList();
}
