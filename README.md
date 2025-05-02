# OOPSQUESTION2
/* Create a simple application with at least two packages:
com.example.geometry and com.example.utils. In the geometry
package, define classes like Circle and Rectangle. In the utils
package, create a Calculator class that can compute areas of these
shapes. */

package Com.Example;

public  class Circle {
    private static double radius;
    public Circle( double radius ) {
        this.radius = radius;
    }
    public double getRadius() {
        return radius;
    }

    }

    package Com.Example.Geometry;

public class Rectangle {
    private static double width;
    private static  double length;
    public Rectangle(double width, double length) {
        this.width = width;
        this.length = length;
    }
    public double getWidth() {
        return width;
    }
    public double getLength() {
        return length;
    }

}

package Com.Example;
public class Calculator {
  public static double Calculate(Circle circle) {
      return Math.PI * circle.getRadius() * circle.getRadius();
  }

 public static double Calculate(Rectangle rectangle) {
     return (rectangle.getWidth() * rectangle.getLength());
 }
    }


    package Com.Example.GEO;

import Com.Example.Calculator;
import Com.Example.Circle;
import Com.Example.Rectangle;

public class CalculatorAreas {
   public static void main(String[] args) {
       Circle circle = new Circle(9.67);
  double circleArea= Calculator.Calculate(circle);
        Rectangle rectangle = new Rectangle(9.67, 9.67);
        double rectangleArea=Calculator.Calculate(rectangle);
        System.out.println(circleArea);
        System.out.println(rectangleArea);

    }
}
