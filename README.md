import javax.swing.JOptionPane;

public class Waynegift {

    public static void main(String[] args) {
        
        // First dialog: ask the user to think of a number
        JOptionPane.showMessageDialog(null, "Think of a number between 1 and 10.");
        
        // Generate a random number from 1 to 10
        int randomNumber = 1 + (int)(Math.random() * 10);
        
        // Second dialog: show the generated number
        JOptionPane.showMessageDialog(null, "The number is " + randomNumber);
        
    }
}

