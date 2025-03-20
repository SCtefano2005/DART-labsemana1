# DART-labsemana1

void main() {
  List<int> numeros = [1, 23, 35, 46, 58, 69, 790, 80, 93, 10];

  int sumpares = numeros.where((num) => num % 2 == 0).fold(0, (a, b) => a + b);
  int sumimpares = numeros.where((num) => num % 2 != 0).fold(0, (a, b) => a + b);

  int sumMenorMayor = numeros.reduce((a, b) => a < b ? a : b) +
                       numeros.reduce((a, b) => a > b ? a : b);

  print("Suma de los pares: $sumpares");
  
  print("Suma de los impares: $sumimpares");
  
  print("Suma del menor y del mayor: $sumMenorMayor");
}
