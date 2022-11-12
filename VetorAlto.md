class VetorAlto
{
	private long[] a;
	private int nElementos;
	//----------------------------------------------------
	public VetorAlto (int max)  //construtor
	{
		a = new long [max];		//criar o vetor
		nElementos = 0;			//não há itens ainda
	}
	//----------------------------------------------------
	public long recupera (int i)
	{
	return a[i];				//recupera um valor no vetor
	}
	//----------------------------------------------------
	public boolean encontrar(long chave)	//encontra valor especifico
	{
		int j;
		for (j=0; j<nElementos; j++)		//para cada elemento
			if(a[j] == chave)				//encontrou item?
				break;						//sair do loop antes do fim
		if(j == nElementos)					//foi ao fimal?
			return false;					//sim, nao encontrei
		else
			return true;					//não, encontrei
	}
	//----------------------------------------------------
	public void inserir(long value)			//colocar elemento no vetor
	{
		a[nElementos] = value;				//inseri elemento
		nElementos++;						//incrementa +1
	}
	//-----------------------------------------------------
	public boolean excluir(long value)
	{
		int j;
		for(j=1; j<nElementos; j++)			//encontrar elemento que quer excluir
			if(value == a[j])
				break;
		if(j==nElementos)					//não encontrou
			return false;
		else								//encontrou
		{
			for(int k=j; k<nElementos; k++)	//mover elementos para frente
				a[k] = a[k+1];
			nElementos--;					//decrementar
			return true;
		}
	}
	//----------------------------------------------------
	public void display()
	{
		for(int j=0; j<nElementos; j++)
			System.out.print(a[j]+ " ");		//para cada elemento
		System.out.println("");				//display
	}
}

