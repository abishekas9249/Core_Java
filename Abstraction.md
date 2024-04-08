### Abstraction
  *Abstraction in Java is one of the key principles of object-oriented programming (OOP). It involves simplifying complex reality by modeling classes appropriate to the problem, and working at the most relevant level of inheritance for a given aspect of the problem.*

```java
abstract class Car{
    abstract void drive();
    abstract void fly();
    void playMusic(){
        System.out.println("Play Heavy Music I am a Car Interface.");
    }
}
abstract class Ambassador extends Car{
    @Override
    void drive() {
        System.out.println("Ambassador Car Can Drive");
    }
}
class FlyingCar extends Ambassador{
    @Override
    void fly() {
        System.out.println("Flying Car can Fly Higher.");
    }

    @Override
    void drive() {
        super.drive();
        System.out.println("Flying Car can Drive Faster.");
    }
}
public class AbstractClass {
    public static void main(String[] args) {
        Car car=new FlyingCar();
        car.playMusic();
        car.drive();
        car.fly();
    }
}
```
## Note:

* An Abstract Class Must be Extended and Implemented in a subclass with
all the method Implementation or else we will get an error.
* You can not create object for abstract class in Common.
* If an abstract method from a abstract class is not implemented in a subclass  then
the subclass can be made abstract later can be implemented in another subclass.

* Critical Cases
  * Abstract class can contain only Normal Methods-->True.
  * Abstract class can contain only Abstract Methods-->True.
  * Abstract class can contain Abstract Methods and Non-Abstract Methods-->True.
  * Abstract class can contain One or More Abstract Methods and One or More Non-Abstract Methods-->True.

* Abstract class can contain Constructors


