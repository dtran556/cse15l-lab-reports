# Lab 2 Report
By Daniel Tran

## Part 1: Creating a Web Server:
In this part of the lab, we are creating a web server called ```StringServer``` and has the ability to add strings to a list and will return the list of strings added and display them on to the server.
The server will keep track of the requests to enter a string using this: ```/add-message?s=<string>```.

For example if you wanted to add a string saying "Hello" you do this: ```/add-message?s=Hello``` and it would look like this : 

You can add another string to it and it would look like this: 

My code is shown below:
```import java.io.IOException;
import java.net.URI;
import java.util.*;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    int num = 0;
    ArrayList<String> masterList = new ArrayList<String>();

    public String handleRequest(URI url) {
        System.out.println("Path: " + url.getPath());
        String input = "";
        if (url.getPath().contains("/add")) {
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")) {
                if (!masterList.contains(parameters[1])) {
                    masterList.add(parameters[1]);
                }
            }
            for (int i = 0; i < masterList.size(); i++) {
                input +=  masterList.get(i) + "\n";
            }
            return input;
        }
        if (url.getPath().contains("/search")) {
            String[] parameters = url.getQuery().split("=");
            ArrayList<String> temp = new ArrayList<String>();
            // check if it contains store into temp list and return the temp
            if (parameters[0].equals("s")) {
                for (int i = 0; i < masterList.size(); i++) {
                    if (masterList.get(i).equals(parameters[1])) {
                        temp.add(parameters[1]);
                    }
                }
                if (!temp.isEmpty()) {
                    return temp.toString();
                }
            }
            return "404 Not Found!";
        }
        return "";
    }

    public class SearchEngine {
        public static void main(String[] args) throws IOException {
            if (args.length == 0) {
                System.out.println("Missing port number! Try any number between 1024 to 49151");
                return;
            }

            int port = Integer.parseInt(args[0]);

            Server.start(port, new Handler());
        }
    }
}
```
I derived this code from the NumberServer.java file, the method for the search engine is called ```handleRequest``` and its only arguement is to pass in a url. You can pass in any value after the ```/add-message?s=``` and it will work as the code will process t in as a string.


## Part 2: De-Bugging:
In lab three I tested the reverseInPlace method which is supposed to reverse an array of ints. However we were not getting it for some inputs.
The failure inducing input:
for the test I decided to try an array of length four which was ```{12,48,24,55}``` and it should return ```{55,24,48,12}```

The input that does not induce a failure:
When the array was length one it would not induce a failure:

The symptoms of the :
The symptom of this bug would be that it just does not properly reverse the array.

Before the fixes:
```static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
 ```

After the fixes (Fixes were conducted with my lab partner during lab 3):
```int[] newArr = new int [arr.length]; 
    for (int i = 0; i < arr.length; i++) {
      newArr[i] = arr[arr.length - i - 1];
    }
    
    for (int i = 0; i < newArr.length; i++) {
      arr[i] = newArr[i];
    }
 ```
The fix fixes the issue because I introduced a new array of the same length which would update the values of ```newArr``` at each index instead of replacing at the indices of ```arr```. This was because ```arr[i[``` was being updated during each iteration of the loop and the values in newArray remained the same.
