# Exercicio-3-AF
Exercicio 3 AF Media de alunos 


1. C == 1
2. Soma == 0
3. Enquanto C <= 6 Faça
4.  Ler(Q[C])
5. Soma <- Soma+ Q[C]
6. C <- C + 1
7 Fim enquanto
8. Media <- Soma/6
9. Exibir ('A média é',Media)


package media_aluno_vet;

import java.util.Scanner;

public class med_alu_vet {

	public static void main(String[] args) {
		Scanner batman = new Scanner(System.in);
//Formando variaveis   
		int n = 6; // Colocando valor nas variaveis
		int s[] = new int[n];// Colocando  matriz
		int i;
		// Mostrar na tela
		System.out.println("informe Quantos Alunos tem nas Salas:");
		// Codigo para criar repetição repetição
		for (i = 0; i < n; i++) {
			System.out.printf("Sala %d: ", (i + 1), n);
			s[i] = batman.nextInt();// colocando valores digitado pelo usuario

		}

		int soma = 0;
		int menor = s[0];
		int maior = s[0];

		for (i = 0; i < n; i++) {
			soma = soma + s[i];
			if (s[i] < menor) // criando condição
				menor = s[i];
			if (s[i] > maior)
				maior = s[i];

		}
		// Espaço de 1 linha
		System.out.println();
		System.out.printf("\nMedia de Alunos = %d\n", (soma / n));
		System.out.println();
		batman.close();
		for (i = 0; i < n; i++) {
			if (s[i] < (soma / n))
				System.out.printf("Sala %d = %2d <--- Sala com MENOR numero da media de alunos\n", i, s[i]);
			else if (s[i] > (soma / n))
				System.out.printf("Sala %d = %2d <--- Sala com MAIOR numero da media de alunos\n", i, s[i]);

		}

	}

}


![image](https://user-images.githubusercontent.com/103973613/173458099-00b1e0c1-561c-460f-9d8c-dbc4b1d43e89.png)
