# parcial3corte
parcial tercer corte pinateria

package duban.monroy;

import static duban.monroy.promedio.preciofinalp;
import static duban.monroy.promedio.precioproducto1;
import static duban.monroy.promedio.precioproducto2;
import static duban.monroy.promedio.precioproducto3;
import static duban.monroy.promedio.precioproducto4;
import static duban.monroy.promedio.precioproducto5;
import java.util.Scanner;


    public  class Trabajotercercorte {
         static double preciofinal;
         
        
       
        
        public static void main(String[]args){
            Scanner scaner= new Scanner(System.in);
            
            int opcion;
            do{
                System.out.println("----BIENVENIDO A LA PIÑATERIA---- ");
                System.out.println("escoja una opcion");
                System.out.println("1--SUMA");                           /*tenemos el menu para todas las opciones*/
                System.out.println("2--MULTIPLICACION ");
                System.out.println("3--PROMEDIO ");
                System.out.println("4--SALIR ");
                
                opcion=scaner.nextInt();
            }  while (opcion<1 || opcion >4);
            
            switch(opcion){
                case 1 -> {
                    suma suma1= new suma();          /*tenemos la suma*/
                    suma1.getClass();
                    
                    System.out.println("resultado de la suma es "+preciofinal);
                 }
                case 2 -> {
                    multiplicacion multiplicacion1 = new multiplicacion();             /*tenemos la multipliacion*/
                    multiplicacion1.getClass();
                    System.out.println("resultado de la multiplicacion es "+preciofinal);
                    
                    
                   
                 }
                
                case 3 -> {
                    promedio promedio1 = new promedio();                       /*tenemos el promedio*/
                    promedio1.getClass();
                    System.out.println("resultado del promedio es "+preciofinal);
                    preciofinalp=(float)(precioproducto1+precioproducto2+precioproducto3+precioproducto4+precioproducto5)/5;

                    
                   
                 }
               
               
                   
                case 4 -> System.out.println("gracias");                                              
            }
        
           
            
         
          
        
       
        }
        
        
    }


    
    package duban.monroy;

import java.util.*;


public class suma {
    static double precioproducto1,precioproducto2,precioproducto3,precioproducto4,precioproducto5,preciofinals;
   
    
    
public static void main(String[]args)
{
    
    
    System.out.println("por favor introdusca el precio para su suma");
    
    Scanner Teclado  = new Scanner(System.in);
    
    System.out.println("dijite el primer precio");
    precioproducto1=Teclado.nextDouble();
    
    System.out.println("dijite el segundo precio");
    precioproducto2=Teclado.nextDouble();
   
    System.out.println("dijite el tercer precio");
    precioproducto3=Teclado.nextDouble();
    
    System.out.println("dijite el cuarto precio");
    precioproducto4=Teclado.nextDouble();
    
    System.out.println("dijite el quito precio");
    precioproducto5=Teclado.nextDouble();
    
    preciofinals=(float)precioproducto1+precioproducto2+precioproducto3+precioproducto4+precioproducto5;
    
    
    System.out.println("resultado de la suma es "+preciofinals);
   
    }
    
}
public class multiplicacion {
    static double precioproducto1,precioproducto2,precioproducto3,precioproducto4,precioproducto5,preciofinalm;
   
    
    
public static void multiplicacion(String[]args)
{
  
    
    System.out.println("por favor introdusca el precio para su multiplicacion");
    
    Scanner Teclado  = new Scanner(System.in);
    
    System.out.println("dijite el primer precio");
    precioproducto1=Teclado.nextDouble();
    
    System.out.println("dijite el segundo precio");
    precioproducto2=Teclado.nextDouble();
   
    System.out.println("dijite el tercer precio");
    precioproducto3=Teclado.nextDouble();
    
    System.out.println("dijite el cuarto precio");
    precioproducto4=Teclado.nextDouble();
    
    System.out.println("dijite el quito precio");
    precioproducto5=Teclado.nextDouble();
    
    preciofinalm=(float)precioproducto1*precioproducto2*precioproducto3*precioproducto4*precioproducto5;
    
    
    System.out.println("resultado de la multiplicacion es "+preciofinalm);
   
    }
    
}
package duban.monroy;

import java.util.*;


public class promedio{
    static double precioproducto1,precioproducto2,precioproducto3,precioproducto4,precioproducto5,preciofinalp;
   
    
   
public static void main(String[]args)
{
  
    
    System.out.println("por favor introdusca el precio para saber su promedio");
    
    Scanner Teclado  = new Scanner(System.in);
    
    System.out.println("dijite el primer precio");
    precioproducto1=Teclado.nextDouble();
    
    System.out.println("dijite el segundo precio");
    precioproducto2=Teclado.nextDouble();
   
    System.out.println("dijite el tercer precio");
    precioproducto3=Teclado.nextDouble();
    
    System.out.println("dijite el cuarto precio");
    precioproducto4=Teclado.nextDouble();
    
    System.out.println("dijite el quito precio");
    precioproducto5=Teclado.nextDouble();
    
    preciofinalp=(float)(precioproducto1+precioproducto2+precioproducto3+precioproducto4+precioproducto5)/5;
    
    
    System.out.println("resultado del promedi "+preciofinalp);
   
    }
    


