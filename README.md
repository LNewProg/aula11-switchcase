// Programa de um menu de aluguel de motos.




#include <iostream>
#include <locale.h>

#define cabeca cout<<"############### MOTORS BIKE RENTAL ################\n    Nós temos a moto que mais combina com você!\n\n\n"
using namespace std;

int main (){
	setlocale(LC_ALL, "Portuguese");
	
	int opc=0;
	char restart='n';
	
	inicio:
	system("cls");
	
	cabeca;
	
	cout<<"[1]Fat boy\n[2]Fat bob\n[3]Vulcan\n\n";
	
	cout<<"Digite o número equivalente à moto de sua escolha: ";
	cin>>opc;
	
	switch(opc){
		case 1:
			system("cls");
			cabeca;
			cout<<"\n                  Ótima escolha!\n\n A Fat boy realmente é a moto perfeita para seu destino!";
			break;
		case 2:
			system("cls");
			cabeca;
			cout<<"\n                  Ótima escolha!\n\n A Fat bob realmente é a moto perfeita para seu destino!";	
			break;
		case 3:
			system("cls");
			cabeca;
			cout<<"\n                  Ótima escolha!\n\n A Vulcan realmente é a moto perfeita para seu destino!";
			break;
		default:
			system("cls");
			cabeca;
			cout<<"\n\nOpção inválida, deseja tentar novamente?[S/N] ";
			cin>>restart;
			if(restart=='s'||restart=='S') {
				goto inicio;	
			}else{
				cout<<"\n\nObrigado pela preferência, volte sempre!";
				system("pause");
			}
	}
	
	
	
	
	return 0;
}
