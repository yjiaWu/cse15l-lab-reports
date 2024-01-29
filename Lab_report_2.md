`
import java.io.IOException;
import java.net.URI;
class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated byhttp://localhost:4000
    // various requests.
    public int size = 10;
    private static final int expand = 2; 
    public int num = 0;
    public String[] information = new String[size];

    public String handleRequest(URI url) {
         if (url.getPath().contains("/add-message")) {
            String[] messages = url.getQuery().split("&");
            String[] param1 = messages[0].split("=");
            String[] param2 = messages[1].split("=");
            if(size == information.length){
                int newsize = size * expand; 
                String[] newinform = new String[newsize];
                for(int i = 0; i < size; i++) {
                    newinform[i] = information[i];
                }
                information = newinform;
                size = newsize; 
            }
            if (param1[0].contains("s")&&param2[0].contains("user")) {
                String message = param2[1] + ": " + param1[1];
                information[num] = message;
                num += 1; 
                String returnmsg = "";
                for(int i = 0; i < num; i++){
                    if(information[i] != null){
                        returnmsg += information[i] + "\n";
                    }

        
                }
                return returnmsg;

            }
            
            return "right path but wrong query";
            
    
        }
    
        return "404 Not Found!";
        
    }
}

class ChatServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
`
![image](Output1.png)<br>


