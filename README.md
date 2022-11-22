//NO ARG CONSTRUCTOR

class Main {
    int i;
    Main(){
        i = 5;
        System.out.println("Constructor is called");
    }
    public static void main(String[] args) {
        Main obj = new Main();
        System.out.println("Value of i: " + obj.i);
    }
}
==================================================================================
class Main {

  String languages;

  // constructor accepting single value
  Main(String lang) {
    languages = lang;
    System.out.println(languages + " Programming Language");
  }

  public static void main(String[] args) {

    // call constructor by passing a single value
    Main obj1 = new Main("Java");
    Main obj2 = new Main("Python");
    Main obj3 = new Main("C");
  }
}

====================================================================================
class Main {

  int a;
  boolean b;

  public static void main(String[] args) {

    // A default constructor is called
    Main obj = new Main();

    System.out.println("Default Value:");
    System.out.println("a = " + obj.a);
    System.out.println("b = " + obj.b);
  }
}

===============================================================================================
different types of methods
public class Main{
    public static void findEvenOdd(int num) {
        if(num%2==0)
            System.out.println(num+" is even");
        else
            System.out.println(num+" is odd");
    }
    public static void main(String[] args){
        findEvenOdd(23);
        System.out.print("The maximum number is: " + Math.max(9,7));
    }
}  

==========================================================================================================
// MULTI-LEVEL INHERITANCE
class Food {
    public void item() {
        System.out.println("Item: Food");
    }
}
class Beverages extends Food {
    public void category() {
        System.out.println("Category - Beverages");
    }
}
class Coffee extends Beverages {
    public void drink (){
        System.out.println("Drink - Coffee");
    }
}
public class Inheritance {
    public static void main(String[] arguments) {
        Coffee  wt= new Coffee ();
        wt.item();
        wt.category();
        wt.drink();
    }
}
=====================================================================================================================================
//ARRAYS SORTING

import java.util.Arrays;
class SORTING {
    public static void main(String args[])
    {
        int[] arr = { 5, -24, 23, 7, 87, -52, 1007 };
        System.out.println("UNSORTED ARRAY :  ");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        Arrays.sort(arr);
        System.out.println("\n SORTED ARRAY(ASCENDING): ");
        for (int num : arr) {
            System.out.print(num + " ");
        }
    }
}

========================================================================================================================
Create new file

import java.io.File;   
class FileInfo {  

    public static void main(String[] args) {  

        // Creating file object  

        File f0 = new File("D:FileOperationExample.txt");  

        if (f0.exists()) {  

            // Getting file name  

            System.out.println("The name of the file is: " + f0.getName());  

   

            // Getting path of the file   

            System.out.println("The absolute path of the file is: " + f0.getAbsolutePath());     

   

            // Checking whether the file is writable or not  

            System.out.println("Is file writeable?: " + f0.canWrite());    

   

            // Checking whether the file is readable or not  

            System.out.println("Is file readable " + f0.canRead());    

   

            // Getting the length of the file in bytes  

            System.out.println("The size of the file in bytes is: " + f0.length());    

        } else {  

            System.out.println("The file does not exist.");  
            
            f0.delete()

        }  

    }  

}
