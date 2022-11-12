#1) Ler 10 elementos de uma matriz tipo vetor e apresentá-los.

import java.util.Scanner;

public class Exer01 {
	
	public static void main(String[] args) 
	{
		VetorAlto vetor = new VetorAlto(10);
		Scanner input = new Scanner(System.in);
		int valor;
		System.out.println("Entre com 10 valores para o vetor");
		for(int i=0; i<10; i++) 
		{
			valor = input.nextInt();
			vetor.inserir(valor);
		}
		vetor.display();
	}
}

