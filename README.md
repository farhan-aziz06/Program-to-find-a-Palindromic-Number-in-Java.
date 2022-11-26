# Program-to-find-a-Palindromic-Number-in-Java.
Write a Java program to check the given number is palindromic or not?



import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
       
        Scanner console = new Scanner(System.in);
        System.out.println("Enter a palindromic Number: ");
        int Number = console.nextInt();
        int r, Sum=0;
        int tempNumber= Number;
        while (Number>0){
             r = Number%10;

            Sum = (Sum*10)+r;
            Number= Number/10;
        }

        if (Sum==tempNumber){
            System.out.println("Entered Number: "+ tempNumber+" is a Palindromic Number: " + Sum);
        }else
            System.out.println("Entered Number: "+ tempNumber+ " is Not a Palindromic Number:" + Sum);

    }
}
