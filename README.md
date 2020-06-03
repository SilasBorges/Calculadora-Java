# Calculadora-Java
Esse é um programa desenvolvido em java, o programa simula uma calculadora fazendo calculos básicos .

package calculadora;

import java.util.Scanner;

public class Principal {

	public static void main(String[] args) {
		
		Scanner sc = new Scanner(System.in);
		
		char operacao;
		double valor1,valor2, total = 0;
		
		System.out.println("***********  CALCULADORA ***********\n");
		System.out.println("Qual operação deseja fazer ? \n para soma digite + \n para subtração digite - \n para multiplicação digite * \n para divisao digite / \n\n");
		operacao = sc.nextLine().charAt(0);
		
		System.out.println("Qual o primeiro valor:");
		valor1 = sc.nextDouble();
		
		System.out.println("Qual o segundo valor:");
		valor2 = sc.nextDouble();
		
		
		if(operacao == '+' ) {
			
			total = valor1 + valor2;
			
		}else if(operacao == '-') {
			
			total = valor1 - valor2;
			
		}else if(operacao == '*') {
			
			total = valor1 * valor2;
			
		}else if(operacao == '/') {
			
			total = valor1 / valor2;
			
		}else {
			System.out.println("Operação invalida!");
		}
		System.out.println("O resultado é: " + total);
	}

}
