package base64sagwapo;

import java.util.Base64;
public class Base64sagwapo {

    
    public static void main(String[] args) {
        String name = "James Harvey Gwapo";
        String encoder = Base64.getEncoder().encodeToString(name.getBytes());
        System.out.println("ENCODED STRING \n" + encoder);
        String encoded = "SmFtZXMgSGFydmV5IEd3YXBv";
         byte [] actualbyte = Base64.getDecoder().decode(encoded);  
         String actualstring = new String (actualbyte);
         System.out.println("DECODED:\n"+ actualstring);
     
    }
    
}
