# Avg-by-while-loops
package com.company;

import jdk.swing.interop.SwingInterOpUtils;

import java.util.Scanner;

public class Main
{
    public static void main (String args[])
    {

        Scanner in = new Scanner(System.in);
        float sum=0;
        float grade=0;
        int count=0;


        while (grade!=-1)
        {

            System.out.println("Enter your grade #" + (count+1) + " : ");
            grade= in.nextFloat();
            if(grade!=-1) {
                sum += grade;
                count++;
            }
        }
        System.out.println("Avg = "+sum/count);
    }
}
