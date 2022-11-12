#13) Escreva um algoritmo que armazene em um vetor os 100 primeiros números ímpares. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer13 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(100);
		int cont=0;
		while(true) {
			if(cont==1)
				vetor.inserir(cont);
			else if((cont%2)==1)
				vetor.inserir(cont);
			cont++;
			if(cont==200)
				break;
		}
		vetor.display();
	}

}
