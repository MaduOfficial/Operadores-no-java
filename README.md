# Operadores-no-java

Anotações sobre Operadores

                                                           Operadores (Aritiméticos, Lógicos e Relacionais)

Tipos de operadores
.Operadores Aritméticos
.Operadores Relacionais
.Operadores Lógicos
.Operadores de Assignment
.Precedência

                                                                       O que são operadores

.Símbolos que solicitam ao compilador realizar alguma operação, então pode ser a soma de dois números, a subtração, a divisão, a multiplicação, lendo duas
variáveis ou dois valores o compilador sabe que dependêndo do operador se for uma só uma subtração, multiplicação, divisão qualquer operação que necessita
ser executada.

                                                                      Operadores Aritméticos

Os Operadores Aritméticos nós já estamos bem acostumados, na escola a gente sempre viu os Operadores Aritméticos que seriam os operadores de fazer soma,
subtração, multiplicação e divisão.

                                    __________________________________________________
                                    |                     |                          |
                                    |      Operadores     |       Descrição          |
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          +          |  adição (e mais unário)  |
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          -          |subtração (e menos unário)|
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          *          |       multiplicação      |
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          /          |          divisão         |
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          %          |           módulo         |
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          ++         |incremento (pos ou pré fix|
                                    |_____________________|__________________________|
                                    |                     |                          |
                                    |          --         |decremento (pos ou pré fix|
                                    |_____________________|__________________________|


int resultado = 1 + 2;
System.out.println(resultado);

resultado = resultado - 1;
System.out.println(resultado);

resultado = resultado * 2;
System.out.println(resultado);

resultado = resultado / 2;
System.out.println(resultado);

resultado = resultado + 8;

resultado = resultado % 7;
System.out.println(resultado);

A gente também pode útilizar o operador de + de adição para fazer concatenar Strings para poder juntar Strings.

String primeiroString = "Esta é";
String segundaString = "Uma String concatenada.";
String terceiraString = primeiraString + segundaString;
System.out.println(terceiraString);

A gente também pode utilizar o de imcremento e decremento.

resultado = + 1;
System.out.println(resultado);

resultado = --;
System.out.println(resultado);

resultado = ++;
System.out.println(resultado);

resultado = -resultado;
System.out.println(resultado);
boolean success = false;

System.out.println(success);

System.out.println(!success);

e esse é mais um exemplo de incremento e decremento

int i = 3;
i++;
// output 4
System.out.println(i);
++i;
// output 5
System.out.println(i);
// output 6
System.out.println(++i);
// output 6
System.out.println(i++);
// output 7
System.out.println(i);



_
package OperadoreAritimeticosTeste;

public class OperadoreAritimeticosTeste1 {

	public static void main(String[] args) {
		
		int resultado = 1 + 2;
		System.out.println(resultado);
		
		resultado = resultado - 1;
		System.out.println(resultado);
		
		resultado  = resultado * 2;
		System.out.println(resultado);
		
		resultado = resultado / 2;
		System.out.println(resultado);
		
		resultado = resultado + 8;
		System.out.println(resultado);
		
		resultado = resultado % 7;
		System.out.println(resultado);
		
		String primeiroNome = "Esta é";
		String segundoNome = "uma String concatenada";
		String terceiroNome = primeiroNome + segundoNome;
		System.out.println(terceiroNome);
		
		resultado = resultado + 1;
		System.out.println(resultado);
		
		resultado++;
		System.out.println(resultado);
		
		//5
		System.out.println(resultado++);
		//mesma coisa que
		//System.out.println(++resultado);
		//resultado = resultado + 1;
		//resultado += 1;
		
        System.out.println(++resultado);
		//mesma coisa que
        //resultado += 1;
        //System.out.println(++resultado);
        
        resultado--;
        System.out.println(resultado);
        
        System.out.println(resultado--);
        System.out.println(--resultado);
	}

}


Console:
2
4
2
10
3
Esta ?uma String concatenada
4
5
5
7
6
6
4

                                                                      Operadores Relacionais

Os operadores relacionais são aqueles que a gente usa para fazer comparação.
                                                   __________________________________________________
                                                   |                     |                          |
                                                   |      Operador       |       Descrição          |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         ==          |         igual a          |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         !=          |      diferente de        |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          >          |        maior que         |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          <          |        menor que         |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         >=          |    maior ou igual que    |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         <=          |    menor ou igral que    |
                                                   |_____________________|__________________________|


package com.madu.OperadoresRelacionaisTeste;

public class OperadoresRelacionaisTeste1 {

	public static void main(String[] args) {
		
		int valor1 = 1;
		int valor2 = 2;
		
		System.out.println("valor1 == valor2: " + (valor1 == valor2));
		System.out.println("valor1 != valor2: " + (valor1 != valor2));
		System.out.println("valor1 > valor2: " + (valor1 > valor2));
		System.out.println("valor1 >= valor2: " + (valor1 >= valor2));
		System.out.println("valor1 < valor2: " + (valor1 < valor2));
		System.out.println("valor1 <= valor2: " + (valor1 <= valor2));
   }

}

Console:
valor1 == valor2: false
valor1 != valor2: true
valor1 > valor2: false
valor1 >= valor2: false
valor1 < valor2: true
valor1 <= valor2: true

                                                                  Operadores Lógicos

Os operadores lógicos a gente útiliza bastante.
                                                   __________________________________________________
                                                   |                     |                          |
                                                   |      Operador       |       Descrição          |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          &          |           AND            |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          |          |            OR            |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          ^          |           XOR            |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         ||          |    OR curto circuito     |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |         &&          |   AND curto circuito     |
                                                   |_____________________|__________________________|
                                                   |                     |                          |
                                                   |          !          |           NOT            |
                                                   |_____________________|__________________________|

                                                                   Tabela Verdade
                                                   ___________________________________________________________________
                                                   |          |          |          |          |          |          |
                                                   |    a     |    b     |    a&b   |   a|b    |   a^b    |    !a    |
                                                   |__________|__________|__________|__________|__________|__________|
                                                   |          |          |          |          |          |          |
                                                   |  falso   |  falso   |  falso   |  falso   |  falso   |verdadeiro|
                                                   |__________|__________|__________|__________|__________|__________|
                                                   |          |          |          |          |          |          |
                                                   |verdadeiro|  falso   |  falso   |verdadeiro|verdadeiro|  falso   |
                                                   |__________|__________|__________|__________|__________|__________|
                                                   |          |          |          |          |          |          |
                                                   |  falso   |verdadeiro|  falso   |verdadeiro|verdadeiro|verdadeiro|
                                                   |__________|__________|__________|__________|__________|__________|
                                                   |          |          |          |          |          |          |
                                                   |verdadeiro|verdadeiro|verdadeiro|verdadeiro|  falso   |  falso   |
                                                   |__________|__________|__________|__________|__________|__________|

package com.madu.OperadoresLogicosTeste;

public class OperadoresLogicosTeste1 {

	public static void main(String[] args) {
        
		int valor1 = 1;
		int valor2 = 2;
		
		boolean resultado1 = (valor1 == 1) && (valor2 == 2);
		System.out.println("valor1 é 1 AND valor2 é 2 - resultado: " + resultado1);
		
		boolean resultado2 = (valor1 == 1) || (valor2 == 2);
		System.out.println("valor1 é 1 OR valor2 é 2 - resultado: " + resultado2);
		
		boolean verdadeiro = true;
		boolean falso = false;
		System.out.println(verdadeiro && falso);
		System.out.println(verdadeiro || falso);
		System.out.println(verdadeiro ^ falso);
		System.out.println(!verdadeiro || falso);
	}

}

Console:
valor1 ? 1 AND valor2 ? 2 - resultado: true
valor1 ? 1 OR valor2 ? 2 - resultado: true
false
true
true
false

                                                                 Curto circuito

package com.madu.CurtoCircuito;

public class CurtoCircuitoTeste1 {

	public static void main(String[] args) {
		
		boolean verdadeiro = true;
		boolean falso = false;
		boolean resultado1 = falso & 
				verdadeiro;
		boolean resultado2 = falso && 
				verdadeiro;
		System.out.println(resultado1);
		System.out.println(resultado2);
	}

}

Console:
false
false


                                                   ________________________________________________________
                                                   |                     |                                |
                                                   |      Operador       |       Precedência              |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |       postfix       |      expr++ expr--             |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |       unário        |  ++expr --expr +expr -expr~!   |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |     multiplicado    |           */%                  |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |       aditivo       |            +-                  |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |        shift        |         << >> >>>              |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |      relacional     |   < > <= >+ instanceof         |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |      igualdade      |         '=='!=                 |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |     bitwise AND     |            &                   |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |bitwise exclusivo OR |            ^                   |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |bitwise inclusivo OR |            |                   |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |     lógico AND      |            &&                  |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |     lógico OR       |            ||                  |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |      ternário       |            ?:                  |
                                                   |_____________________|________________________________|
                                                   |                     |                                |
                                                   |     assignment      |=+= _= *= /= %= &= ^= |= <<= >>=|
                                                   |_____________________|________________________________|

package com.madu.CurtoCircuito;

public class CurtoCircuitoTeste1 {

	public static void main(String[] args) {
		
		boolean verdadeiro = true;
		boolean falso = false;
		boolean resultado1 = falso & 
				verdadeiro;
		boolean resultado2 = falso && 
				verdadeiro;
		System.out.println(resultado1);
		System.out.println(resultado2);
		
		int resultado = 1 + 1 - 1 + 1 * 1 / 1;
		System.out.println(resultado);
	}

}

Console:
false
false
2
