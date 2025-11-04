import java.util.Scanner;

class Employee {
    int id;
    String name;
    String position;
    double salary;

    Employee(int id, String name, String position, double salary) {
        this.id = id;
        this.name = name;
        this.position = position;
        this.salary = salary;
    }
}

public class EmployeeManagementSystem {
    private static final int MAX_EMPLOYEES = 100;
    private static Employee[] employees = new Employee[MAX_EMPLOYEES];
    private static int employeeCount = 0;
    private static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        int choice;

        do {
            System.out.println("\n=== Employee Management System ===");
            System.out.println("1. Add Employee");
            System.out.println("2. View Employees");
            System.out.println("3. Update Employee");
            System.out.println("4. Delete Employee");
            System.out.println("5. Exit");
            System.out.print("Enter your choice: ");
            choice = getIntInput();

            switch (choice) {
                case 1 -> addEmployee();
                case 2 -> viewEmployees();
                case 3 -> updateEmployee();
                case 4 -> deleteEmployee();
                case 5 -> System.out.println("Exiting program...");
                default -> System.out.println("Invalid choice! Try again.");
            }
        } while (choice != 5);
    }

    private static void addEmployee() {
        if (employeeCount >= MAX_EMPLOYEES) {
            System.out.println("Employee list is full!");
            return;
        }

        System.out.print("Enter Employee ID: ");
        int id = getIntInput();

        System.out.print("Enter Name: ");
        String name = scanner.nextLine();

        System.out.print("Enter Position: ");
        String position = scanner.nextLine();

        System.out.print("Enter Salary: ");
        double salary = getDoubleInput();

        employees[employeeCount++] = new Employee(id, name, position, salary);
        S
