import javax.swing.JOptionPane;

public class SequentialDialogs {

    public static void main(String[] args) {
        // First Dialog Box: Takes user input
        String name = JOptionPane.showInputDialog(
            null, 
            "Enter your name:", 
            "Step 1 of 2", 
            JOptionPane.QUESTION_MESSAGE
        );

        // Check if the user entered a name or clicked Cancel
        if (name != null && !name.trim().isEmpty()) {
            // Second Dialog Box: Displayed after the first one is dismissed
            JOptionPane.showMessageDialog(
                null, 
                "Hello, " + name + "! Welcome to NetBeans.", 
                "Step 2 of 2", 
                JOptionPane.INFORMATION_MESSAGE
            );
        } else {
            // Alternative Second Dialog Box if the user canceled or left it blank
            JOptionPane.showMessageDialog(
                null, 
                "No name provided. Operation canceled.", 
                "Step 2 of 2", 
                JOptionPane.WARNING_MESSAGE
            );
        }
    }
}
