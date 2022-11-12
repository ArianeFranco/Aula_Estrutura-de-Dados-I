#6) Escreva um algoritmo que armazene em um vetor todos os números inteiros de 0 a 50. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer06 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(51);
		int count=0;
		while (true) {
			vetor.inserir(count);
			count=count+1;
					if (count==51)
						break;
		}
		vetor.display();

	}

}
