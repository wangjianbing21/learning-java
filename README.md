# learning-java
class Animal{
  private String name;
   Animal(String name){
   this.name = name;
   }
public void enjoy(){
   System.out.println("动物叫声......");
   }
}

class Dog extends Animal{
   private String furcolor;
   Dog(String n,String c){
   super(n);
   furcolor = c;
   }
public void enjoy(){
   System.out.println("狗叫声......");
   }
}

class Cat extends Animal{
   private String eyescolor;
   Cat(String q,String e){
   super(q);
   eyescolor = e;
   }
public void enjoy(){
   System.out.println("猫叫声......");
  
   }
}

class Lady{
   private String name;
   private Animal pet;
   Lady(String name,Animal pet){
   this.name = name;
   this.pet = pet;
   }
public void mypet(){
   pet.enjoy();
   }
}
public class TestDuoTai{
   public static void main(String[] args){
	   Cat c1 = new Cat("harry","blue");
	   Dog d1 = new Dog("bigyellow","yellow");
	   Lady l1 = new Lady("l1",c1);
	   Lady l2 = new Lady("l2",d1);
           l1.mypet();
	   l2.mypet();
	  // System.out.println(l1.name);
	   // System.out.println(c1.name);
	 




}
}
