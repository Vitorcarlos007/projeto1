#include <stdio.h>

int main() {
    char nome1[10];
    char nome2[10];
    int idade1;
    int idade2;
    int nascimento1;
    int nascimento2;
    int diado_nascimento1;
    int aniversario1;  // mês do aniversário 1
    int aniversario2;  // mês do aniversário 2
    float peso1;
    float peso2;

    printf("Digite o primeiro nome: ");
    scanf("%s", nome1);
    printf("Nome 1: %s\n", nome1);

    printf("Digite o segundo nome: ");
    scanf("%s", nome2);
    printf("Nome 2: %s\n", nome2);

    printf("Digite sua idade: ");
    scanf("%d", &idade1);
    printf("idade1: %d\n", idade1);

    printf("Digite sua idade: ");
    scanf("%d", &idade2);
    printf("idade2: %d\n", idade2);

    printf("Digite o ano do seu nascimento: ");
    scanf("%d", &nascimento1);
    printf("nascimento1: %d\n", nascimento1);

    printf("Digite o ano do seu nascimento: ");
    scanf("%d", &nascimento2);
    printf("nascimento2: %d\n", nascimento2);
    
    printf("Digite o dia do nascimento 1: ");
    scanf("%d", &diado_nascimento1);
    printf("diado_nascimento1: %d\n", diado_nascimento1);

    printf("Digite mes do aniversario: ");
    scanf("%d", &aniversario1);
    printf("aniversario1: %d\n", aniversario1);
    
    printf("Digite mes do aniversario: ");
    scanf("%d", &aniversario2);
    printf("aniversario2: %d\n", aniversario2);

    printf("digite o seu peso: ");
    scanf("%f", &peso1);
    printf("peso1, %f\n", peso1);

    printf("digite seu peso: ");
    scanf("%f", &peso2);
    printf("peso2, %f\n", peso2);



    if (idade1 > idade2) {
        printf("idade1 e mais velho\n");
    } else {
        printf("idade2 e mais novo\n");
    }

    if (peso1 > peso2) {
        printf("peso1 e mas pesado que o peso2\n");
    }   else {
        printf("peso2 e mas leve que o peso1");
    }

    return 0;
}
