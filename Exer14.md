#14) Escreva um algoritmo que armazene em um vetor o quadrado dos números ímpares no intervalo fechado de 1 a 20. Após isso, o algoritmo deve imprimir todos os valores armazenados.

public class Exer14 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetor = new VetorAlto(10);
		for(int i=1;i<20;i=1+2)
			vetor.inserir(i*i);
		vetor.display();
	}

}
