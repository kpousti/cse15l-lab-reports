Part 1: StringServer Web Server:
import java.io.IOException;
import java.net.URL;

class handler implements URLHandler {
    String s ="";

    public String handlerequest(Url url){
        if(ur.path().equals("/")){
            return s;
        }

        else if(url.path().contains("/add-message")){
            String[] parameters = url.getQuery().split("=");
            if(parameters[0].equals("s")){
                s=s.concat("\n"+parameters[1]);
                return string.format(s);

        }
    }
    return "404 Not Found";
}
}

class StringServer{
    public static void main(String[] args) throws IOException{
        if (args.length==0){
            System.out.println("Missing port number! Try again with a number between 1 and 9999");
            return;
        }

        int port= Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
}

