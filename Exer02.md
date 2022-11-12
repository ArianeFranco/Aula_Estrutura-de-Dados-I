#2) Ler 8 elementos em uma matriz A tipo vetor. Construir uma matriz B de mesma dimensão com os elementos da matriz A multiplicados por 3. O elemento B[1] deverá ser implicado pelo elemento A[1] * 3, e assim por diante.

public class Exer02 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		VetorAlto vetorA = new VetorAlto(8);
		VetorAlto vetorB = new VetorAlto(8);
		Scanner input  = new Scanner (System.in);
		int valor;
		System.out.println("Entre com 8 valores para o vetor");
		for(int i=0;i<8;i++) {
			valor = input.nextInt();
			vetorA.inserir(valor);
		}
		for(int i=0;i<8;i++) {
			vetorB.inserir(vetorA.recupera(i)*3);
			
	}
		System.out.println("Vetor A");
		vetorA.display();
		System.out.println("Vetor B");
		vetorA.display();
}
}
