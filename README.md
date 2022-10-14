# ejercicio4

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {


        System.out.println("el valor es:");

//Usando un if, crear una condición que compare si la variable
// numeroIf es positivo, negativo, o 0.
        int num1 = 0;


        if (num1 > 0) {


            System.out.println("positivo");
        } else {

            if (num1 < 0) {

                System.out.println("negativo");
            } else {
                System.out.println("neutro");
            }

        }
//Crea un bucle While, este bucle tendrá que tener como condición que la variable numeroWhile sea inferior a 3,
// el bloque de código que tendrá el bucle deberá:
//
//Incrementar el valor de la variable en uno cada vez que se ejecute.
//
//Mostrarlo por pantalla cada vez que se ejecute.

        int contador =0;

        while (contador<3) {

            System.out.println(contador);


            contador = contador +1;

        }
//Para el bucle Do While, deberás crear la misma estructura que en el While,
// pero solo se debe ejecutar una vez.

        int n;

        Scanner ob=new Scanner(System.in);

        do {
            System.out.println("ingrese un valor");

            n=ob.nextInt();
        }while(n<1 || n>100);

//Para el bucle For, crea una variable numeroFor, esta variable tendrá como valor 0 y su condición será que la variable sea igual o menor que 3,
// se irá incrementando en 1 su valor cada vez que se ejecute y deberá mostrarse por pantalla.

        for (int i = 0; i <= 3; i++) {

            System.out.println("el valor es " + i);
        }
//Por último, para el Switch, deberás crear la variable estacion, y distintos case para las cuatro estaciones del año. Dependiendo del valor de la variable estacion se deberá mandar un mensaje por consola informando de la estación en la que está.
// También habrá que poner un default para cuando el valor de la variable no sea una estación.
      
      
      int estacion=2;
        String nombreestacion;
                switch(estacion){
                    case 1: nombreestacion="invierno";
                    break;
                    case 2: nombreestacion="primavera";
                    break;
                    case 3: nombreestacion="verano";
                    break;
                    case 4: nombreestacion="otoño";
                    break;
                    default: nombreestacion="no existe";
                    break;
                }
                System.out.println("la estacion del año es " + nombreestacion);
    }
}
