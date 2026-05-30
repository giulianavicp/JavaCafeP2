# Avaliação P2 - Linguagem de Programação - Prof. Bruno Zolotareff
Nomes:
Catarina Eri Nakatani
Giuliana Victoria Pedrassi

Máquina de café com POO - Respostas:

Como foi aplicado os três paradigmas da Programação Orientada a Objeto
Abstração:  A abstração está na criação da classe Drink. Definimos que, para o funcionamento do sistema da máquina, qualquer bebida precisa ter duas propriedades fundamentais: sabor e valor. Por ser uma classe abstrata (public abstract class Drink), ela serve como um conceito ou um molde geral, impedindo que o sistema crie um "Drink" genérico sem uma receita específica.

Herança: Esse pilar é aplicado na linha public class Cafe extends Drink. Isso significa que a classe concreta Cafe é uma extensão (uma filha) da classe Drink. Por conta disso, Cafe não precisa declarar novamente as variáveis sabor e valor pois ela já as possui automaticamente. No construtor de Cafe, o comando super(sabor, valor) é utilizado para enviar esses dados diretamente para a classe mãe inicializar.

Encapsulamento: Na classe Drink, as variáveis são definidas como private (private double valor;). Isso impede que a classe MaquinaCaffe altere o preço fazendo algo como cafe.valor = -5.00. Para modificar ou ler o preço, o sistema é obrigado a usar os métodos setValor() e getValor(). Isso garante que o controle do dado permaneça sob as regras da própria classe.

Explicando o Polimorfismo
O polimorfismo permite que o objeto Cafe seja referenciado e tratado de formas diferentes na classe principal, dependendo do que o sistema precisa no momento e garante que o sistema consiga interagir com o objeto Cafe olhando apenas para a característica necessária naquele instante, tornando o código mais seguro.

