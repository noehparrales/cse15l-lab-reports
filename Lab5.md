# Part 1 
## Student Post
__Title__
File not found error message 
__Category__
Labs




```
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class h {

    public static void main(String[] args) {
        h fileSystem = new h();
        fileSystem.readFromFile("input.txt");
    }

    public void readFromFile(String fileName) {
        try {
            File file = new File(fileName);
            Scanner scanner = new Scanner(file);

            while (scanner.hasNextLine()) {
                String line = scanner.nextLine();
                processLine(line);
            }

            scanner.close();
        } catch (FileNotFoundException e) {
            System.out.println("File not found: " + e.getMessage());
        }
    }

    public void processLine(String line) {
        // Simulate processing each line, but introduce a bug
        System.out.println(line + " " + generateMysteriousCharacters());
    }

    public String generateMysteriousCharacters() {
        // Simulate a bug causing unexpected characters
        return "\u001B[31m???\u001B[0m";
    }
}
```
