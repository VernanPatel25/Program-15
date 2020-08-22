import java.util.Scanner;
class EMPLOYEE
{
    double base, sal;
    int hra;
    void input()
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Dear Employee, enter your basic salary: ");
        base = sc.nextDouble();
        System.out.println("Dear Employee, your HRA : ");
        hra = sc.nextInt();
    }
    void calc()
    {
        sal = base + (50*hra)/100;
    }
    void display()
    {
        System.out.println("Dear Employee, your current salary : "+sal);
    }
    public static void main()
    {
        EMPLOYEE obj = new EMPLOYEE();
        obj.input();
        obj.calc();
        obj.display();
    }
}
