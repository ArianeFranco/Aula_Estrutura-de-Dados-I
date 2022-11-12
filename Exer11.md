#11) Escreva um algoritmo que armazene em um vetor todos os números múltiplos de 5, no intervalo fechado de 1 a 500. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer11 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(500);
		int count=0;
		while(true) {
			if(count==1)
				vetor.inserir(count);
			else if((count%5)==0)
				vetor.inserir(count);
			count++;
			if(count==501)
				break;
		}
		vetor.display();
	}

}
