#include <stdio.h>

int main() {
    char nome1[10];
    char nome2[10];
    int idade1, idade2;
    int nascimento1, nascimento2;
    int diado_nascimento1;
    int aniversario1, aniversario2;
    float peso1, peso2;
    int opcao;

    // Exibe menu
    printf("Menu Principal\n");
    printf("1. Iniciar cadastro\n");
    printf("2. Sair\n");

    // Lê a opção do usuário
    printf("Escolha uma opção: ");
    scanf("%d", &opcao);

    switch (opcao) {
        case 1: 
            printf("Iniciando cadastro...\n");
            break;

        case 2:
            printf("Saindo do programa...\n");
            return 0; // Encerra o programa aqui

        default:
            printf("Opção inválida. Tente novamente.\n");
            return 1; // Também encerra, já que opção inválida
    }

    // Cadastro da primeira pessoa
    printf("Digite o primeiro nome: ");
    scanf("%s", nome1);

    printf("Digite sua idade: ");
    scanf("%d", &idade1);

    printf("Digite o ano do seu nascimento: ");
    scanf("%d", &nascimento1);

    printf("Digite o dia do nascimento: ");
    scanf("%d", &diado_nascimento1);

    printf("Digite o mês do aniversário: ");
    scanf("%d", &aniversario1);

    printf("Digite o seu peso: ");
    scanf("%f", &peso1);

    // Cadastro da segunda pessoa
    printf("Digite o segundo nome: ");
    scanf("%s", nome2);

    printf("Digite sua idade: ");
    scanf("%d", &idade2);

    printf("Digite o ano do seu nascimento: ");
    scanf("%d", &nascimento2);

    printf("Digite o mês do aniversário: ");
    scanf("%d", &aniversario2);

    printf("Digite seu peso: ");
    scanf("%f", &peso2);

    // Comparação de idades
    if (idade1 > idade2) {
        printf("%s é mais velho que %s.\n", nome1, nome2);
    } else if (idade2 > idade1) {
        printf("%s é mais velho que %s.\n", nome2, nome1);
    } else {
        printf("%s e %s têm a mesma idade.\n", nome1, nome2);
    }

    // Comparação de pesos
    if (peso1 > peso2) {
        printf("%s pesa mais que %s.\n", nome1, nome2);
    } else if (peso2 > peso1) {
        printf("%s pesa mais que %s.\n", nome2, nome1);
    } else {
        printf("%s e %s têm o mesmo peso.\n", nome1, nome2);
    }

    return 0;
}
