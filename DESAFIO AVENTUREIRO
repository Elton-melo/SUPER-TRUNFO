#include <stdio.h>

int main() {
    // Declarando variáveis para armazenar as informações do jogo
    char estado1[2], estado2[2];  // Mudando para string de 2 caracteres
    char cidade1[10], cidade2[10];
    char nome1[50], nome2[50];
    unsigned int populacao1, populacao2;
    float area1, area2;
    float pib1, pib2;
    int ponto_turistico1, ponto_turistico2;
    float pib_per_capita1, pib_per_capita2;
    float densidade_populacional1, densidade_populacional2;
    double super_poder1, super_poder2;

    // Criando interação com o usuário para cadastrar as cartas 1
    printf("**** Bem-vindo ao jogo Super Trunfo ****\n\n");
    
    printf("\n----Primeira carta----\n");

    printf("Digite o estado (A a H): ");
    scanf("%s", estado1);
    printf("Digite o código da cidade (1 a 4): ");
    scanf("%s", cidade1);
    getchar();  // Usado para remover o newline do buffer
    printf("Digite o nome da cidade: ");
    fgets(nome1, sizeof(nome1), stdin);
    printf("Digite a população da cidade: ");
    scanf("%u", &populacao1);
    printf("Digite a área da cidade (em km²): ");
    scanf("%f", &area1);
    printf("Digite o PIB da cidade: ");
    scanf("%f", &pib1);
    printf("Digite o número de pontos turísticos da cidade: ");
    scanf("%d", &ponto_turistico1);

    // Criando interação com o usuário para cadastrar as cartas 2
    printf("\n----Segunda carta----\n");

    printf("Digite o estado (A a H): ");
    scanf("%s", estado2);
    printf("Digite o código da cidade (1 a 4): ");
    scanf("%s", cidade2);
    getchar();  // Usado para remover o newline do buffer
    printf("Digite o nome da cidade: ");
    fgets(nome2, sizeof(nome2), stdin);
    printf("Digite a população da cidade: ");
    scanf("%u", &populacao2);
    printf("Digite a área da cidade (em km²): ");
    scanf("%f", &area2);
    printf("Digite o PIB da cidade: ");
    scanf("%f", &pib2);
    printf("Digite o número de pontos turísticos da cidade: ");
    scanf("%d", &ponto_turistico2);

    // Cálculos da densidade, PIB per capita e super poder
    densidade_populacional1 = populacao1 / area1;
    pib_per_capita1 = pib1 / populacao1;
    super_poder1 = populacao1 + area1 + pib1 + ponto_turistico1 + pib_per_capita1 + (1 / densidade_populacional1);

    densidade_populacional2 = populacao2 / area2;
    pib_per_capita2 = pib2 / populacao2;
    super_poder2 = populacao2 + area2 + pib2 + ponto_turistico2 + pib_per_capita2 + (1 / densidade_populacional2);

    // Menu de escolha de atributo
    int opcao;
    do {
        printf("\nEscolha o atributo para comparação:\n");
        printf("1 - População\n");
        printf("2 - Área\n");
        printf("3 - PIB\n");
        printf("4 - Pontos turísticos\n");
        printf("5 - Sair\n");
        printf("Opção: ");
        scanf("%d", &opcao);

        switch (opcao) {
            case 1:
                // Comparação de população
                if (populacao1 > populacao2) 
                    printf("Cidade 1 (%s) venceu na População!\n", nome1);
                else if (populacao1 < populacao2) 
                    printf("Cidade 2 (%s) venceu na População!\n", nome2);
                else 
                    printf("Empate na População!\n");
                break;
            case 2:
                // Comparação de área
                if (area1 > area2) 
                    printf("Cidade 1 (%s) venceu na Área!\n", nome1);
                else if (area1 < area2) 
                    printf("Cidade 2 (%s) venceu na Área!\n", nome2);
                else 
                    printf("Empate na Área!\n");
                break;
            case 3:
                // Comparação de PIB
                if (pib1 > pib2) 
                    printf("Cidade 1 (%s) venceu no PIB!\n", nome1);
                else if (pib1 < pib2) 
                    printf("Cidade 2 (%s) venceu no PIB!\n", nome2);
                else 
                    printf("Empate no PIB!\n");
                break;
            case 4:
                // Comparação de pontos turísticos
                if (ponto_turistico1 > ponto_turistico2) 
                    printf("Cidade 1 (%s) venceu nos Pontos turísticos!\n", nome1);
                else if (ponto_turistico1 < ponto_turistico2) 
                    printf("Cidade 2 (%s) venceu nos Pontos turísticos!\n", nome2);
                else 
                    printf("Empate nos Pontos turísticos!\n");
                break;
            case 5:
                printf("Saindo do jogo...\n");
                break;
            default:
                printf("Opção inválida. Tente novamente.\n");
        }
    } while (opcao != 5);

    return 0;
}
