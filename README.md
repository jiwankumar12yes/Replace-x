# Replace-x
package recursion2;
import java.util.*;
public class remove_x {
    public static void main(String args[]){
        // System.out.println("Hello");
        Scanner s=new Scanner(System.in);
        System.out.println("enter a string to remove x");
        String str=s.next();
        System.out.println(Remove(str));
    }
    public static String Remove(String str){
        if(str.length()==0){
            return str;
        }
        String ans="";
        if(str.charAt(0)!='x'){
            ans=ans+str.charAt(0);
        }
        String smallans=Remove(str.substring(1));
        return ans+smallans;
    }
    
}

