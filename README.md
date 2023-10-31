# Hw5
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
