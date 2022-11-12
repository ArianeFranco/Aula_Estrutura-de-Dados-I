#4) Ler 15 elementos de uma matriz A do tipo vetor. Construir uma matriz B de mesmo tipo, observando a seguinte lei de formação: “ Todo elemento de B deverá ser o quadrado do elemento de A correspondente”. Apresentar as matrizes A e B.

public class Exer04 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetorA = new VetorAlto(15);
		VetorAlto vetorB = new VetorAlto(15);
		Scanner input = new Scanner (System.in);
		Random aleatorio = new Random();
		for (int i=0;i<15;i++)
			vetorA.inserir(aleatorio.nextInt(10));
	for(int i=0;i<15;i++) {
		vetorB.inserir(vetorA.recupera(i)*vetorA.recupera(i));
	}
	System.out.println("Vetor A");
	vetorA.display();
	System.out.println("Vetor B");
	vetorB.display();
	}
	}
