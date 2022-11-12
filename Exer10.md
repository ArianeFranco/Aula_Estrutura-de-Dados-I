#10) Escreva um algoritmo que armazene em um vetor todos os números inteiros de 200 a 100 (em ordem decrescente). Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer10 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(101);
		int count = 200;
		while (true) {
			vetor.inserir(count);
			count--;
			if (count==99)
					break;
		}
		vetor.display();
	}

}

