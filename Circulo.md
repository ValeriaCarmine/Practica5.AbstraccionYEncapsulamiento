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
public class Circulo {
    static float PI = 3.1416f;
    private float radio;

    public Circulo() {
    }

    public Circulo(float radio) {
        this.radio = radio;
    }

    public float getRadio() {
        return radio;
    }

    public void setRadio(float radio) {
        if(radio<0)
            this.radio = 0;
        else       
        this.radio = radio;
    }
    
    public float perimetro(){
        return 2* PI * radio;
    }
    
    public float area(){
        return PI * radio * radio;
    }

    @Override
    public String toString() {
        return "Circulo{" + "radio=" + radio + '}';
    }
    
}
