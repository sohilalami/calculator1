# calculator1

Mijn naam is Sohil Alami en dit is mijn opdracht

import java.util.Scanner;

public class Main {

    public static  void main(String[] args) {


        Scanner scan = new Scanner(System.in);


        System.out.println("vul het eerste getal in");

        int getal_1= scan.nextInt();

        System.out.println("vul het tweede getal in");
        int getal_2= scan.nextInt();

        System.out.println("kies een manier om jouw cijfers te berekenen.");
        System.out.println("kies A voor optellen.");
        System.out.println("kies B voor aftrekken.");
        System.out.println("kies C voor vermenigvuldigen.");
        System.out.println("kies D voor delen.");


        char choice = scan.next().charAt(0);

        if(choice == 'a') {
            System.out.println("het antwoord is " + optellen(getal_1, getal_2));
        }
        if(choice == 'b') {
            System.out.println("het antwoord is " +  aftrekken(getal_1, getal_2));
        }
        if(choice == 'c') {
            System.out.println("het antwoord is " +  vermenigvuldigen(getal_1, getal_2));
        }
        if(choice == 'd') {
            System.out.println("het antwoord is " +  delen(getal_1, getal_2));
        }




    }

    private static int optellen(int num_1, int num_2) {

        int antwoord_1 = (num_1 + num_2);

        return antwoord_1;


    }

    private static int aftrekken(int num_1, int num_2) {

        int antwoord_2 = (num_1 - num_2);

        return antwoord_2;

    }

    private static int vermenigvuldigen(int num_1, int num_2) {



        int antwoord_3 = (num_1 * num_2);

        return antwoord_3;



    }

    private static int delen(int num_1, int num_2) {

        int antwoord_4 = (num_1 / num_2);


        return antwoord_4;



    }
}
