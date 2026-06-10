//variable:-

//      1.var 
//      2.let 
//      3.const

// 1.var :- allowed to same name, diffrent value , value types

//  example:-

    // var x=10;
    // var x=10;
    // console.log(x);

    // var x="rohit";
    // var x="rahul";
    // console.log(x);

    // var x="rohit";
    // var y="10";
    // console.log(x);

// 2.let :- not allowed to same name, allowed to diffrent value type, value

// example:

    // ex:1
    //        let x=20;
    //        y=30;
    //        console.log(x);

    //ex:2
    //       let myname="rahul";
    //       myname="rohit patel";
    //       console.log(myname);

    //ex:3
    //       let x="10";
    //       x="rohit"
    //       console.log(x);

// 3.const :- not allowed to same name,value type,value

    //ex.:-1
    // const x="rohit";  
    // console.log(x);

    //ex.:-2
    // const x="rahul";  
    //       y="patel";
    // console.log(x+y);

//-------------------------------------------------------------------------------------- 
  
//operators:-

///there are mainly 4 types of operators

 //     1.arithmetic 
 //     2.logical 
 //     3.comparison
 //     4.assignment

    //1.arthicmetic...[+,-,*,/]

    //example:-
        // var x=2;
        // var y=3;
        // console.log("add:",x+y);
        // console.log("sub:",x-y);
        // console.log("mul:",x*y);
        // console.log("div:",x/y);

    //2.logical...[||,&&]

    // example:-
                
        // let x=12;
        // let  y=1;
        // if(x==12 || y==1 )
        // {
        //     console.log("this number");
        // }
        // if(x==12 && y==1 )
        // {
        //     console.log("there number");
        // }

    //3.comparison....[==,===,!=(not equal),!==,>,<,>=,<=]

    //example:-

        // let a=10;
        // let b=5;

        // console.log(a>b);
        // console.log(a<b);
        // console.log(a==b); 
        // console.log(a!=b);

    //4.assignment....[=,+=,-=,*=,/=]

    //example:-

        // let balance=1000;

        // balance+=500;
        // console.log(balance);
        // balance-=500;
        // console.log(balance);
        // balance*=500;
        // console.log(balance);
        // balance/=500;
        // console.log(balance);

//----------------------------------------------------------------------------------------------------

// condition :- if, if else , else if else..

    // if :-
    // ex:-

        //  let a=20;
        //  let b=30;
        //      if(a<b)
        //      {
        //      console.log("b is max");
        //      }

    // if else :-
    // ex:-

        // let a=20;
        // let b=30;
        //     if(a<b)
        //          {
        //             console.log("b is max");
        //          }
        //     else
        //         {
        //          console.log("a is max");
        //         }

     // else if else:-
     //ex:-

            // let a=75;

            // if(a>=90)
            // {
            //     console.log("grade a");
            // }
            // else if(a>=70)
            // {
            //     console.log("grade b");
            // }
            // else
            // {
            //     console.log("grade c");
            // }

//------------------------------------------------------------------------------------------------------

    //loop :- for, while, do while

    //for:-
    //ex:-

        // for(let i=1;i<=5;i++)
        //     { 
        //         console.log(i);
        //     }

    //ex:-

        //  for(let i=1;i<=5;i++){
        //       console.log("*".repeat(i))
        //  }

    //ex:-

        //  for(let i=5;i>=1;i--)
        //   {
        //     console.log("*".repeat(i));
        //   }


    // while :-
    //ex:-

        //    let i=3;
        //     while(i<=7)
        //     {
        //         console.log(i);
        //         i++;
        //     }

    //ex:-

        //    let i=1;
        //    while(i<=10){
        //        console.log(i);
        //        i++
        //    }

    // do while:-
    //ex:-

        // let i=1;
        //  do{
        //     console.log(i);
        //     i++;
        //  } while(i<=5);
    
    //ex:-

        //  let i=6;
        //  do{
        //    console.log(i);
        //    i++
        //     }
        //  while(i<=10);

//----------------------------------------------------------------------------------------------

// data types :

// 1. string 2.number 3.bigint 4.boolean (true,false) 5.undefined 6.null 7.symbol 8.object(non-primitive data types)

// 1.string :-

     //  let name ="krisha";
    //  console.log(name);

//2.number :-

    // let x=10;
    // console.log(x);

//3.bigint:-
 
     // let bigint=20056840281858;
     //console.log(bigint);

//4.boolean :-

    //let age=20;
    //console.log(age<=15);
  
//5.undefined  :-

    //let age;
    //age=20;
    //console.log(age);

//6.null :-

    // let user = null;
    // console.log(user);

//7.symbol:-

    // let id1=symbol("id");
    // let id2=symbol("id");   
    // console.log(id1===id2)

//8.object:-  

    // let person={
    //     name:"krisha",
    //     age:20,
    //     city:"jamnagar"
    // };
    // console.log(person);

//-----------------------------------------------------------------------------------------------------

    // array:-
    // array collect multiple value in one variable

    // example:-
     
    // let fruits = ["apple","mango","graps"];

    // console.log(fruits[0]);
    // console.log(fruits[1]);
    // console.log(fruits[2]);
    // console.log(fruits.length);

//--------------------------------------------------------------------------------------------------

//OOPs (object-oriented programing):-
//        ~ it is based on object.
//        ~ it follows bottom-up programming approach.
//        ~ it is based on real world.
//        ~ it provides data hiding so it is very secure.
//        ~ it provides reusability feature.

//class:-
//        ~ a class ia a collection of objects.
//        ~ class don't consume any space in the memory.
//        ~ a large number of object can be created using the same class.therefore,
//          class is considered as the blueprint for the object.
//        ~ it is user defined data type that as a template for creating objects of
//          the identical type.

//object:-
//          ~ an object is real world entity which have properties and functionalities.
//          ~ object is also called an instance of class.
//          ~ object take some space in memory.
//          ex:- fruit is class and its object are mengo,apple,banana

// following are the basic feature of OOPs:-
//      1.inheritance
//      2.abstraction
//      3.encapsulation
//      4.polymorphimsm

// 1.inheritance:-
//                ~ there are four types of inheritance..
//                      - single inheritance
//                      - hierarchical inheritance
//                      - multi-level inheritance
//                      - multiplpe inheritance
//                      - hybrid inheritance
//
//      - single inheritance :-
//                            ~ single inhetitance is object-oriented programming concept 
//                              where a class inherits properties and method from only one
//                              parent(base)class.
//
//                            ~ diagram :-
//                                          Animal
//                                             |                                    
//                                             v                       
//                                            dog
//
//      - hierarchical inheritance :-
//                                 ~ where multiple child class inherit from a single parent class.
//
//                                 ~ diagram :-
//                                               Animal
//                                                /  \
//                                              dog   cat
//
//      - multi-level inheritance :-
//                                  ~ where a class inherits from another deried class, forming a
//                                    chain of inheritance.
//
//                                  ~ diagram :-
//                                                manager              
//                                                  |    
//                                                  v
//                                               employee
//                                                  |     
//                                                  v
//                                                person
//
//      - multiplpe inheritance :-
//                                ~ where a class inherits from more than one parent class.
//
//                                ~ diagram :-
//                                              class A   class B
//                                                   ^      ^
//                                                  /        \      
//                                                   class C
//
//        - hybrid inheritance :-
//                                ~ hybrid inherits is a combination of two or more types of heritance.
//
//                                ~ diagram :-
//                                                   A
//                                                 /   \
//                                                B     C  
//                                                 \   /
//                                                   D 
//----------------------------------------------------------------------------------------------------------
// 2.abstraction :-
//                 ~ abstraction is the process of hiding unnecessary details and showing only the essential
//                  features to the usser.
//
//                 ~ abstract class is that class which contains abstract method. 
//
//                 ~ abstract methods are those method which have only declaration not the implementation.     
//
//                 ~ an abstract class is declared with abstract keyword. 
//
//----------------------------------------------------------------------------------------------------------
//3.encapsulation :-
//                  ~ encapsulation means wrapping data(variables)and method(function)into a single unit(class)
//                    and protecting the data from direct access.  
//
//---------------------------------------------------------------------------------------------------------
//4.polymorphimsm :-
//                  ~ the same method or function can behave differently for different object.
//
// example :-
//
//          class Dog extends Animal {
//              sound() {
//                   console.log("Dog barks");
//                  }
//                }
//          class Cat extends Animal {
//               sound() {
//                    console.log("Cat meows");
//                  }
//                }
//           const dog = new Dog();
//           const cat = new Cat();
//           dog.sound();
//           cat.sound();
//
// types of polymorphism:-
//                          1. compile time polymorphism
//                          
//                          2. run time polymorphism
//
//1. compile time polymorphism:- 
//                              ~ Compile-Time Polymorphism means the method/function is decided 
//                                 at compile time. It is usually achieved using Method Overloading.
//
//     function overloading:-
//                          ~ Function Overloading means having multiple functions with the same name 
//                             but different parameters.
//
//2. run time polymorphism :-
//                           ~ Runtime Polymorphism means the method that will run is decided while 
//                              the program is running.
//
//      function overriding :-
//                             ~ Runtime Polymorphism means the method that will run is decided 
//                               while the program is running.
//
//---------------------------------------------------------------------------------------------------------
// what is static function? :-
//                          ~ a static function is a function that belongs to a class itself 
//                            rather than to an object (instance) of the class.
//
//what is virtual functions? :-
//                            ~ a virtual function is a function in C++ that allows runtime polymorphism.
//                              It lets a derived class override a function of the base class, 
//                              and the correct function is called based on the actual object type. 
//
//what is pure virtual function?:-
//                              ~ a Pure Virtual Function is a virtual function that has no implementation 
//                                in the base class and must be overridden inthe derived class.
//
//what is constructor?:-
//                      ~ a constructor is a special function of a class that is automatically called
//                       when an object is created.  
//
// the types of constructor:-
//                          1. default constructor (a constructor with no parameters)
//                          2. parameterized constructor (a constructor that accepts parameters)
//                          3. copy constructor (creates a new object by copying another object)
//                          4. static constructor 
//                          5. private constructor
//
//what is destructor:-
//                     ~ a Destructor is a special function in C++ that is automatically called 
//                       when an object is destroyed.
//
//shallow copy and deep copy :-
//                            ~ shallow copy : shallow copy copies the values of data members, 
//                                             including memory addresses (pointers).
//
//                            ~ deep copy : A deep copy creates a new memory location and copies 
//                                          the actual data.
//
//in c++ we can pass argument into a function in different ways:-
//                                                              ~ call by value
//                                                              ~ call by reference
//                                                              ~ call by address
//
