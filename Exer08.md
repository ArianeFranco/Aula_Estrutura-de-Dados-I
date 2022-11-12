#8) Escreva um algoritmo que armazene em um vetor todos os números inteiros de 100 a 1 (em ordem decrescente). Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer08 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(100);
		int count = 100;
		while(true){
			vetor.inserir(count);
			count--;
			if(count==0)
				break;
		}
		vetor.display();

	}

}
