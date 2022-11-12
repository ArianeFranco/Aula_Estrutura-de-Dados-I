#12) Escreva um algoritmo que armazene em um vetor todos os números pares do intervalo fechado de 1 a 100. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer12 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(100);
		int cont=0;
		while(true) {
			if(cont==0)
				vetor.inserir(cont);
			else if((cont%2)==0)
				vetor.inserir(cont);
			cont++;
			if(cont==101)
				break;
		}
		vetor.display();
	}

	}
