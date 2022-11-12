#7) Escreva um algoritmo que armazene em um vetor todos os números inteiros do intervalo fechado de 1 a 100. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer07 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(100);
		int count = 1;
		while (true) {
			vetor.inserir(count);
			count++;
			if(count==101)
				break;
		}
		vetor.display();

	}

}
