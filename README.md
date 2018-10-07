# FileReader
import java.io.File;
import java.lang.Thread.State;
import java.util.ArrayList;
import java.util.Scanner;

public class NumberOne {

    public static void main(String[] args) {
    	String keyword[]= {"if","else","int","float","double"};
    	String identifiers[]= {"a","b","c","d","e","f","g","h","i","j","k","l","m"};
    	String operators[]= {"+","-","*","/","%"};
    	String logicalOperator[]= {">","<"};
    	String others[]= {",",";","()","{}"};
    	ArrayList<String> ar=new ArrayList<>();
    	String s1="if";
    	String s2="else";
    	String s3="int";
    	String s4="float";
    	String s5="double";
    	ar.add(s1);
    	ar.add(s2);
    	ar.add(s3);
    	ar.add(s4);
    	ar.add(s5);
    	
        ArrayList<String> strLi = new ArrayList<>();
        try {
            Scanner sc= new Scanner(new File("C:/Users/sajed/Desktop/text.txt"));
            while(sc.hasNextLine()){
                String st= sc.nextLine();
                String[] temp= st.split(" ");
                for(String item : temp){
                 strLi.add(item);
            } 
            }
        } catch (Exception ex) {
            System.out.println("File not found!");
        }
        
//        for(String i: strLi){
//            System.out.println(i);
//        }
    System.out.println(strLi.get(5));
        
      
       
        
        
        
        
        
        
        
        
       
}
    

}
