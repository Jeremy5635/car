/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaObjects;

/**
 *
 * @author jeremy.carpenter
 */
public class Car {
    public int year;
    public String makeModel;
    
    private boolean isEngineRunning;
    private double speed;
    
    public void startEngine(){
        isEngineRunning = true;
        System.out.println("...crank...crank...vroom!");
    }
    
    public void stopEngine(){
        isEngineRunning = false;
        System.out.println("...grblllll....shldunk");
    }
    
    public boolean checkEngineStatus(){
        return isEngineRunning;
    }
    
    public double getCurrentSpeed(){
        return speed;
    }
    
    public double accelerate(int mphIncrease){
        speed = speed + mphIncrease;
        return speed;
    }
    
    public double decelerate(int mphDecrease){
        speed = speed - mphDecrease;
        return speed;
    }
}
