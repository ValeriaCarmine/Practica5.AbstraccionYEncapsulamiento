# Practica5.AbstraccionYEncapsulamiento
POO/Práctica 5. Abstracción y Encapsulamiento


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package poop5;

/**
 *
 * @author Optiplex 780
 */
public class POOP5 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Circulo circulo1 = new Circulo(8);
        System.out.println("rasio cir1 = "+circulo1.getRadio());
        
        Circulo circulo2 = new Circulo();
        System.out.println(circulo2);
        circulo2.setRadio(2);
        System.out.println(circulo2);
        circulo2.setRadio(-10);
        System.out.println(circulo2);
        
        System.out.println("**************EJERCICIO 2****************");
        Persona per1 = new Persona();
        Fecha fnac = new Fecha();
        
        per1.setNombre("Valeria");
        per1.setApellido("Hernandez");
        fnac.setDia(20);
        fnac.setMes(11);
        fnac.setAnio(2001);
        per1.setfNacimiento(fnac);
        System.out.println(per1);
                
        System.out.println("Fecha de nacimiento: "+per1.getfNacimiento().getDia()+"/"+per1.getfNacimiento().getMes()+"/"+per1.getfNacimiento().getAnio());
        System.out.println("Feca nacimiento: "+per1.getfNacimiento());
        
        System.out.println("**************ACTIVIDAD EXTRA****************");
        // creo las personas que estaran dentro del coche con su fecha de nacimiento cada una
        
        Persona persona1 = new Persona();
        Fecha fnac1 = new Fecha();
        Persona persona2 = new Persona();
        Fecha fnac2 = new Fecha();
        Persona persona3 = new Persona();
        Fecha fnac3 = new Fecha();
        Persona persona4 = new Persona();
        Fecha fnac4 = new Fecha();
        
        // Informacion de la persona 1
        persona1.setNombre("Scarlett");
        persona1.setApellido("Hernandez");
        persona1.setLugar("Soy Pasajero 1");
        fnac1.setDia(4);
        fnac1.setMes(5);
        fnac1.setAnio(1996);
        persona1.setfNacimiento(fnac1);
        
        // Informacion de la persona 2
        persona2.setNombre("Dana");
        persona2.setApellido("Hernandez");
        persona2.setLugar("Soy Pasajero 2");
        fnac2.setDia(20);
        fnac2.setMes(11);
        fnac2.setAnio(2001);
        persona2.setfNacimiento(fnac2);
        
        // Informacion de la persona 3
        persona3.setNombre("Norma");
        persona3.setApellido("Rubio");
        persona3.setLugar("Soy copiloto");
        fnac3.setDia(5);
        fnac3.setMes(1);
        fnac3.setAnio(1976);
        persona3.setfNacimiento(fnac3);
        
        // Informacion de la persona 4
        persona4.setNombre("Teodoro");
        persona4.setApellido("Hernandez");
        persona4.setLugar("Soy chofer");
        fnac4.setDia(20);
        fnac4.setMes(6);
        fnac4.setAnio(1972);
        persona4.setfNacimiento(fnac4);
        
        // Despues de tener a las personas hago un coche y les asaigno su lugar 
        Coche coche1 = new Coche();
        coche1.setChofer(persona4);
        coche1.setCopiloto(persona3);
        coche1.setPasajero1(persona1);
        coche1.setPasajero2(persona2);
        
        System.out.println(coche1);
        System.out.println("*********************************************************************************");
   
        System.out.println(coche1.getPasajero1().getNombre()+" Lugar: "+coche1.getPasajero1().getLugar());
        System.out.println(coche1.getPasajero2().getNombre()+" Lugar: "+coche1.getPasajero2().getLugar());
        System.out.println(coche1.getCopiloto().getNombre()+" Lugar: "+coche1.getCopiloto().getLugar());
        System.out.println(coche1.getChofer().getNombre()+" Lugar: "+coche1.getChofer().getLugar());
        System.out.println("*********************************************************************************");
      
        System.out.println("Chofer: "+coche1.getChofer());
        System.out.println("Copiloto: "+coche1.getCopiloto());
        System.out.println("Pasajero 1: "+coche1.getPasajero1());
        System.out.println("Pasajero 2: "+coche1.getPasajero2());
         
         
    }
    
}
