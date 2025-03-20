# DART-labsemana1
ejercicio planteado
void main() {
  List<int> numeros = [1, 23, 35, 46, 58, 69, 790, 80, 93, 10];

  int sumapares = numeros.where((num) => num % 2 == 0).fold(0, (a, b) => a + b);
  int sumaimpares = numeros.where((num) => num % 2 != 0).fold(0, (a, b) => a + b);

  int sumaMenorMayor = numeros.reduce((a, b) => a < b ? a : b) +
                       numeros.reduce((a, b) => a > b ? a : b);

  print("Suma de los pares: $sumapares");
  print("Suma de los impares: $sumaimpares");
  print("Suma del menor y del mayor: $sumaMenorMayor");
}
