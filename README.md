# unidad_2_Actividad_4
/*
A partir de un arreglo que posee N cantidad de promedios de estudiantes colocarlos
en una lista y sacar el promedio global de todos los estudiantes. Se debe verificar
que los elementos que están en la lista son correcto (rango de 0 a 5).
Imprimir todos los promedios y el promedio global. 
*/
package proyecto1;

import java.util.Scanner;

public class Proyecto1 {
    
    public static void main(String[] args) {

        float acumulado=0;
        float notas=0;
        
        System.out.println("las notas deben estar entre 0 y 5");
        // p el la variable donde almacenaremos datos
        Scanner p =new Scanner(System.in );
        System.out.println("ingrese la cant de notas a promediar");
        //cn es la cantidad de notas 
        float cn=p.nextFloat();// aca se repite teniendo en cuenta el numero de notas

        while(acumulado <=cn){
            System.out.println("ingrese la nota numero:"+acumulado);
            float n=p.nextFloat();
            notas +=n;
            acumulado++;
        }
        float promedio=notas/cn;
        System.out.println("El promedio es: "+promedio);
    }
    
}
