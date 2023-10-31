# Hw5-1
```java
abstract class CShape{
    protected String color;
    public void setColor(String str){
        color = str;
    }
    public abstract void show();
}

class CTriangle extends CShape{
    double x1,x2,x3;
    public CTriangle(double a, double b, double c){
        x1=a;
        x2=b;
        x3=c;
    }
   
    public void show() {
       
        System.out.print("color="+color+"  ");
        System.out.print("area="+0.5*x1*x2);
    }
}

public class Main {
   public static void main(String[] args) {
    CTriangle ct = new CTriangle(3, 4, 5);
    ct.setColor("red");
    ct.show();
  }
}
```
# Hw5-2
```java
import java.util.ArrayList;
import java.util.List;

public class Student {
    private String name;
    private List<Course> courses;

    public Student(String name) {
        this.name = name;
        this.courses = new ArrayList<>();
    }

    public boolean addCourse(Course course) {
        if (courses.size() < 10) {
            courses.add(course);
            return true;
        }
        return false;
    }

    public boolean removeCourse(Course course) {
        return courses.remove(course);
    }

    public List<Course> getCourses() {
        return courses;
    }

    // Other getters, setters, and relevant methods
}

public class Course {
    private String courseName;

    public Course(String courseName) {
        this.courseName = courseName;
    }

    // Getters, setters, and other relevant methods
}
```
