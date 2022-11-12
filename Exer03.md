#3) Ler duas matrizes A e B do tipo vetor com 20 elementos. Construir uma matriz C, em que cada elemento de C é a subtração do elemento correspondente de A com B. Apresentar a matriz C.

public class Exer03 {

	public static void main(String[] args) {
		VetorAlto vetorA = new VetorAlto(20);
		VetorAlto vetorB = new VetorAlto(20);
		VetorAlto vetorC = new VetorAlto(20);
		Scanner input = new Scanner (System.in);
		int valor;
		System.out.println("Entre com 20 valores para a matriz");
		for(int i=0;i<20;i++) {
			valor = input.nextInt();
			vetorA.inserir(valor);

		for(int j=0;j<20;j++) {
			valor = input.nextInt();
			vetorB.inserir(valor);

		for(int k=0;k<20;k++);
		vetorC.inserir(vetorA.recupera(i)-vetorB.recupera(j)); }}

	System.out.println("Vetor A");
	vetorA.display();
	System.out.println("Vetor B");
	vetorA.display();
	System.out.println("Vetor C");
	vetorA.display();
	}

}

