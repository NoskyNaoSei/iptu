# dart
class Imovel {
  double area;

  Imovel(this.area);


  String get iptu{
    if (area <= 0) {
      return "300 reais";
    } else if (area <= 50) {
      return "500 reais";
    } else if (area <= 100) {
      return "800 reais";
      } else if (area <= 200) {
      return "1.200 reais";
      } else if (area > 200) {
      return "2.000 reais";
    } else { 
      return "F";
    }
  }
}

void main() {
  var preco = Imovel(300,);

  print('Área Construída: ${preco.area} m2');
  print("Iptu:  ${preco.iptu} ");
