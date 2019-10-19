# Calcolo-Java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
import java.util.Scanner;

/**
 *
 * @author alessio.vampo
 */
public class CalcoloJava {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        int b, h, area, perimetro;
        Scanner tastiera = new Scanner (System.in);
        
        System.out.print("Inserisci la base:  ");
        b = tastiera.nextInt();
        System.out.print("inserire l'altezza");
        h = tastiera.nextInt();
        System.out.println("area"+calcolo(b, h, 'a'));
        System.out.println("perimetro: "+calcolo(b, h, 'p'));    
    }
    public static int calcolo (int b, int h, char c){
    switch (c) {
        case 'p':return 2 * (b + h);
        case 'a':return b * h;
        default : return 0;
    }
    }
}
