//Dikdörtgen Alanı Hesaplayan Fonksiyon
void main() {
  double uzunKenar = 4.76;
  double kisaKenar = 9.54;

  double alan = dikdortgenAlaniHesapla(uzunKenar, kisaKenar);
  print("Dikdörtgenin Alanı: $alan");
}

double dikdortgenAlaniHesapla(double uzunKenar, double kisaKenar) {
  return uzunKenar * kisaKenar;
}


//carp Fonksiyonu ve main Fonksiyonu
void main() {
  int sonuc = carp(5, 3);
  print("Sonuç: $sonuc"); // Sonuç: 20
}

int carp(int a, int b) {
  int multiplyByTwo(int x) {
    return x * 2;
  }

  int result = a;
  for (int i = 1; i < b; i++) {
    result = multiplyByTwo(result);
  }

  return result;
}


//Listeden Eleman Silen Fonksiyon
void main() {
  List<String> myList = ["apple", "banana", "cherry"];
  print("Orijinal Liste: $myList");

  sil(myList, "banana");
  print("Güncellenmiş Liste: $myList");
}

void sil(List<String> list, String item) {
  list.remove(item);
}


//Şekiller Class'ı ve Objeleri
class Sekil {
  String adi;
  Sekil(this.adi);
}

void main() {
  Sekil kare = Sekil("Kare");
  Sekil dikdortgen = Sekil("Dikdörtgen");
  Sekil daire = Sekil("Daire");
  Sekil ucgen = Sekil("Üçgen");
  Sekil elips = Sekil("Elips");

  List<Sekil> sekiller = [kare, dikdortgen, daire, ucgen, elips];

  for (var sekil in sekiller) {
    print(sekil.adi);
  }
}


