package Itheimaday9;


import java.util.ArrayList;
import java.util.Scanner;

public class ArrayListStudent {
    public static void main(String[] args) {
//        定义一个集合
        ArrayList<Student> arrayList = new ArrayList<Student>();
        Scanner sc = new Scanner(System.in);
        for (; ; ) {
            System.out.println("---欢迎来到学生管理系统---");
            System.out.println("1.添加学生");
            System.out.println("2.删除学生");
            System.out.println("3.修改学生");
            System.out.println("4.查看学生信息");
            System.out.println("5.退出");
            System.out.println("请输入你的选择");
            String a = sc.nextLine();
            switch (a) {
                case "1":
                    studentadd(arrayList);
                    break;
                case "2":
                    delete(arrayList);
                    break;
                case "3":
                    set(arrayList);
                    break;
                case "4":
                    show(arrayList);
                    break;
                case "5":
                    System.out.println("谢谢使用");
                    break;
//                   System.exit(0);
                default:
                    System.out.println("输入有误，请重新输入");
                    break;
            }
            if (a.equals("5")) {
                break;
            }
        }
    }

    //    添加学生信息方法
    public static void studentadd(ArrayList<Student> s) {
        Scanner sc = new Scanner(System.in);
        System.out.println("请输入学号");
        String id = sc.nextLine();
        boolean b;
        if (b = panduan(s, id)) {
            System.out.println("学号重复，请重新输入");
        } else {
            System.out.println("请输入姓名");
            String name = sc.nextLine();
            System.out.println("请输入地址");
            String address = sc.nextLine();
            System.out.println("请输入年龄");
            String age = sc.nextLine();
//        创建一个学生对象
            Student a = new Student();
            a.setId(id);
            a.setName(name);
            a.setAddress(address);
            a.setAge(age);
            s.add(a);
            System.out.println("添加学生成功");
        }
    }

    //      删除学生信息方法
    public static void delete(ArrayList<Student> s) {
        Scanner sc = new Scanner(System.in);
        System.out.println("请输入要删除的学生学号");
        String a = sc.nextLine();
        for (int x = 0; x < s.size(); x++) {
            Student b = s.get(x);
            if (b.getId().equals(a)) {
                s.remove(x);
                System.out.println("删除成功");
            } else {
                System.out.println("请输入正确学号");
            }
        }
    }

    //      查看所有学生信息方法
    public static void show(ArrayList<Student> s) {
        if (s.size() == 0) {
            System.out.println("没有学生数据");
        } else {
            System.out.println("学号\t姓名\t地址\t年龄");
            for (int x = 0; x < s.size(); x++) {
                Student arr = s.get(x);
                System.out.println(arr.getId() + "\t\t" + arr.getName() + "\t" + arr.getAddress() + "\t" + arr.getAge() + "岁");
            }
        }
    }
    //      修改学生信息方法
    public static void set(ArrayList<Student> s) {
        Scanner sc = new Scanner(System.in);
        System.out.println("请输入要修改的学号");
        String id = sc.nextLine();
        System.out.println("请输入要修改的名字");
        String name = sc.nextLine();
        System.out.println("请输入要修改的年龄");
        String age = sc.nextLine();
        System.out.println("请输入要修改的地址");
        String address = sc.nextLine();
//        创建学生对象
        Student b = new Student();
        b.setName(name);
        b.setAddress(address);
        b.setAge(age);
        b.setId(id);
        for (int x = 0; x < s.size(); x++) {
            Student c = s.get(x);
            if (c.getId().equals(id)) {
                s.set(x, b);
                System.out.println("修改成功");
            } else {
                System.out.println("您输入的学号有误");
                break;
            }
        }
    }

    //    创建判断方法，判断ID是否重复
    public static boolean panduan(ArrayList<Student> s, String id) {
        for (int x = 0; x < s.size(); x++) {
            Student a = s.get(x);
            if (a.getId().equals(id)) {
                return true;
            }
        }
        return false;
    }
}
 /*       //    创建集合对象
        ArrayList<Student> students = new ArrayList<Student>();
//    创建学生对象
        Student s1 = new Student(01,"小明", 18,"中关村");
        Student s2 = new Student(02,"小红", 20,"紫禁城");
        Student s3 = new Student(03,"蔡徐坤", 21,"煤炭坝");
//将学生添加到集合中
        students.add(s2);
        students.add(s1);
        students.add(s3);
//        调用方法
            bianli(students);
    }
public static void bianli (ArrayList<Student> s){

        for(int a =0 ; a<s.size();a++ ){
         Student arr =s.get(a);
            System.out.print(arr.getName());
            System.out.print(arr.getAge());
            System.out.print(arr.getId());
            System.out.println(arr.getAddress());
        }

}
*/

