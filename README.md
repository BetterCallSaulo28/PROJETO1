import java.util.Scanner;

public class JogoAgentesSecretos {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Pedir informações do jogador
        System.out.println("Bem-vindo ao mundo dos agentes secretos!");
        System.out.print("Por favor, digite seu nome: ");
        String nome = scanner.nextLine();
        System.out.print("Por favor, digite sua idade: ");
        int idade = scanner.nextInt();
        scanner.nextLine(); // Consumir a quebra de linha

        // Introdução à história
        System.out.println("\nOlá, Agente " + nome + ", de " + idade + " anos.");
        System.out.println("Você foi recrutado para uma missão secreta...");

        // Escolha inicial
        System.out.println("\nVocê está diante de uma porta com três botões numerados: 1, 2 e 3.");
        System.out.println("Qual botão você escolhe pressionar?");
        System.out.println("1. Botão 1");
        System.out.println("2. Botão 2");
        System.out.println("3. Botão 3");
        int escolhaInicial = scanner.nextInt();

        // Segunda escolha
        switch (escolhaInicial) {
            case 1:
                escolhaBotao1();
                break;
            case 2:
                escolhaBotao2();
                break;
            case 3:
                escolhaBotao3();
                break;
            default:
                System.out.println("Escolha inválida! Você falhou em seguir as instruções. Missão terminada!");
        }
    }

    public static void escolhaBotao1() {
        System.out.println("\nVocê pressionou o Botão 1 e uma armadilha é acionada.");
        System.out.println("Você foi capturado pelos inimigos. Fim de jogo!");
    }

    public static void escolhaBotao2() {
        System.out.println("\nVocê pressionou o Botão 2 e uma escotilha se abre, revelando um túnel.");
        System.out.println("Você entra no túnel e continua sua missão. Parabéns, Agente!");
    }

    public static void escolhaBotao3() {
        System.out.println("\nVocê pressionou o Botão 3 e uma voz computadorizada pede uma senha.");
        System.out.println("Você digita uma senha e a porta se abre, revelando o objetivo da missão.");
        System.out.println("Missão cumprida, Agente! Você é um herói.");
    }
}
