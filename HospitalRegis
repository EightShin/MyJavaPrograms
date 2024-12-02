import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String regisUsername = "";
        String regisPassword = "";

        // Registration part
        System.out.println("-------- Registration --------");
        System.out.print("Enter a username to register: ");
        regisUsername = sc.nextLine();
        System.out.print("Enter a password to register: ");
        regisPassword = sc.nextLine();
        System.out.println("Registration successful! Please log in.");

        boolean loggedIn = false;

        while (!loggedIn) {
            System.out.println("\n-------- Login --------");
            System.out.print("Enter Username: ");
            String inputUsername = sc.nextLine();
            System.out.print("Enter Password: ");
            String inputPassword = sc.nextLine();

            if (regisUsername.equals(inputUsername) && regisPassword.equals(inputPassword)) {
                loggedIn = true;
                System.out.println("-------- Login Successful --------");
            } else {
                System.out.println("Invalid Username or Password. Please try again.");
            }
        }

        String patientName = "";
        int patientAge = 0;
        String phoneNumber = "";
        String maritalStatus = "";

        boolean running = true;

        while (running) {
            System.out.println("\nSelect an option:");
            System.out.println("1. Enter Patient Name");
            System.out.println("2. Enter Patient Age");
            System.out.println("3. Enter Phone Number");
            System.out.println("4. Enter Marital Status");
            System.out.println("5. Display Patient Information");
            System.out.println("6. Exit");
            System.out.print("Enter your choice: ");

            int choice = sc.nextInt();
            sc.nextLine(); 

            switch (choice) {
                case 1:
                    System.out.print("Enter Patient Name: ");
                    patientName = sc.nextLine();
                    System.out.println("Patient name saved successfully.");
                    break;
                case 2:
                    System.out.print("Enter Patient Age: ");
                    patientAge = sc.nextInt();
                    sc.nextLine(); 
                    System.out.println("Patient age saved successfully.");
                    break;
                case 3:
                    System.out.print("Enter Phone Number: ");
                    phoneNumber = sc.nextLine();
                    System.out.println("Phone number saved successfully.");
                    break;
                case 4:
                    System.out.print("Enter Marital Status (e.g., Single, Married): ");
                    maritalStatus = sc.nextLine();
                    System.out.println("Marital status saved successfully.");
                    break;
                case 5:
                    if (!patientName.isEmpty() && patientAge > 0 && !phoneNumber.isEmpty() && !maritalStatus.isEmpty()) {
                        System.out.println("\n-----------------");
                        System.out.println("Patient Name: " + patientName);
                        System.out.println("Patient Age: " + patientAge);
                        System.out.println("Phone Number: " + phoneNumber);
                        System.out.println("Marital Status: " + maritalStatus);
                        System.out.println("-----------------");
                    } else {
                        System.out.println("Incomplete information. Please make sure to enter all patient details.");
                    }
                    break;
                case 6:
                    System.out.println("Exiting the system...");
                    running = false;
                    break;
                default:
                    System.out.println("Invalid choice. Please try again.");
                    break;
            }
        }

        System.out.println("Program terminated.");
    }
}
