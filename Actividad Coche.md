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
public class Coche {
    private Persona chofer;
    private Persona copiloto;
    private Persona Pasajero1;
    private Persona Pasajero2;

    public Coche() {
    }

    public Coche(Persona chofer, Persona copiloto, Persona Pasajero1, Persona Pasajero2) {
        this.chofer = chofer;
        this.copiloto = copiloto;
        this.Pasajero1 = Pasajero1;
        this.Pasajero2 = Pasajero2;
    }

    public Persona getChofer() {
        return chofer;
    }

    public void setChofer(Persona chofer) {
        this.chofer = chofer;
    }

    public Persona getCopiloto() {
        return copiloto;
    }

    public void setCopiloto(Persona copiloto) {
        this.copiloto = copiloto;
    }

    public Persona getPasajero1() {
        return Pasajero1;
    }

    public void setPasajero1(Persona Pasajero1) {
        this.Pasajero1 = Pasajero1;
    }

    public Persona getPasajero2() {
        return Pasajero2;
    }

    public void setPasajero2(Persona Pasajero2) {
        this.Pasajero2 = Pasajero2;
    }

    @Override
    public String toString() {
        return "Coche{" + "chofer=" + chofer + ", copiloto=" + copiloto + ", Pasajero1=" + Pasajero1 + ", Pasajero2=" + Pasajero2 + '}';
    }
    
    
    
}
