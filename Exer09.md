#9) Escreva um algoritmo que armazene em um vetor todos os números inteiros de 100 a 200. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer09 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(101);
		int count = 100;
		while (true) {
			vetor.inserir(count);
			count++;
			if (count==201)
					break;
		}
		vetor.display();
	}

}

