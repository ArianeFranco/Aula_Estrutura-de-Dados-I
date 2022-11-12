#5) Ler duas matrizes A e B do tipo vetor com 15 elementos cada. Construir uma matriz C.

import java.util.Random;

public class Exer05 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetorA = new VetorAlto(15);
		VetorAlto vetorB = new VetorAlto(15);
		VetorAlto vetorC = new VetorAlto(30);
		Random aleatorio = new Random();
		for(int i=0; i<15;i++) {
			vetorA.inserir(aleatorio.nextInt(100));
			vetorB.inserir(aleatorio.nextInt(100));
			vetorC.inserir(vetorB.recupera(i));
		}
		for(int i=0; i<15;i++) {
			vetorC.inserir(vetorB.recupera(i));
		}
		System.out.println("vetor A:");
		vetorA.display();
		System.out.println("vetor B:");
		vetorB.display();
		System.out.println("vetor C:");
		vetorC.display();
	}

}
