import { PhotoProvider, PhotoView } from 'react-photo-view';
import 'react-photo-view/dist/react-photo-view.css';
import Icon9 from "@components/icons/Icon9";
import {Callout, ThemeSwitch} from 'nextra-theme-docs';
import CalloutCX from "@components/CalloutCX";


<div className="flex nx-justify-between">

    <h1><span className="p-0 sm:p-0 headingGradientTag font-bold text-transparent sm:text-8xl text-[50px] ">Introduction</span></h1>
</div>
<div className="mt-5"></div>
<CalloutCX
    type="info"
    emoji="🎉"
    title="Read This on Github"
    message="This article is available on Github. You can read it there and contribute to it."
    links={[
        { link: 'https://github.com/Subham-Maity/60-Days-Of-OOPs', linkText: 'Github Link' },
        { link: 'https://github.com/Subham-Maity/60-Days-Of-OOPs/issues/new', linkText: 'Any Issue ?' },
    ]}
/>



## ⭐ Introduction


<div className= "mt-3"></div>
<div className="cardTexture5">
    <h1 style={{padding: "8px"}} className = "mb-8 text-center font-bold text-transparent sm:text-4xl text-[25px] tex bg-clip-text bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-sky-700 via-cyan-500 to-neutral-300" align="middle">

        Example of OOPs
    </h1>
    <h11 className="textStyle1 " >

        <p align="center">
            <img style={{ position: "relative" ,opacity: 1 ,borderRadius: "10px" ,overflow: "hidden" , marginTop:"20px" , marginBottom: "20px"}}
                 src="https://media.giphy.com/media/9aCvf5HaQ0ajT7eBF2/giphy.gif"
                 width="450"/>
        </p>

        So imagine you have a YouTube channel and it's filled with lots of videos. These videos are organized into playlists, like a playlist for music videos and a playlist for comedy videos. Each video has its own set of comments and likes.

        Now in OOPs(object oriented programming) we have objects and classes. So in this example,

        All the videos are objects and the class is the Playlist. So, every object means video has its own set of comments and likes. So, in this example, we can say that the comments and likes are the properties of the video object.

        <div className="mt-8"></div>
        <h12 className ="font-bold text-2xl sm:text-4xl align-middle ml-8">Then what is OOPs 😥❓</h12>
        <div className="mb-8"></div>

        <h12 className ="font-bold text-red-500 dark:text-red-200"> Solving a problem using objects is called object-oriented programming. </h12>



    </h11>
</div>

<Callout type ="info" emoji="📝">
    What is DRY Principle ?

    DRY Stands for -> Don't Repeat Yourself

    It means that you should not repeat the same code over and over again. Instead, you should use functions or classes to reuse the code.
    Here's an example to help explain it:

    Example 1:


    <p align="center">
        <img style={{ position: "relative" ,opacity: 1 ,borderRadius: "10px" ,overflow: "hidden" , marginTop:"20px" , marginBottom: "20px"}}
             src="https://media.giphy.com/media/fXnx6vSSrzY92rTONJ/giphy.gif"
             width="250"/>
    </p>

    Imagine you're building a website for a library. On the website, you have a page that shows a list of all the books in the library. You also have a page that shows a list of all the movies in the library. And you have a page that shows a list of all the music albums in the library.

    If you're not following the DRY principle, you might write separate code for each of these pages to display the list of books, movies, and music albums. But that's a lot of repeating code, because the basic idea is the same for all three pages - they all show a list of items.

    Instead, you should create a class, say Item, which will have all the properties and functions related to the items. And then you can create different objects of the class Book, Movie, Music etc.

    So, you create a single class "Item" that has the code to display a list of items. And then you create different objects of the class for books, movies, and music albums. This way, you only have to write the code for displaying a list of items once, and you can reuse it for all three pages.

    Example 2:
    The DRY principle is a programming principle that says "Don't Repeat Yourself." It means that you should avoid writing the same code multiple times in your program.

    Here's an example to help explain it:

    Let's say you have a program that checks if a number is even or odd. Without following the DRY principle, you might write the following code:
```java
public class Main {
    public static void main(String[] args) {
        int num1 = 5;
        if (num1 % 2 == 0) {
            System.out.println(num1 + " is even");
        } else {
            System.out.println(num1 + " is odd");
        }

        int num2 = 6;
        if (num2 % 2 == 0) {
            System.out.println(num2 + " is even");
        } else {
            System.out.println(num2 + " is odd");
        }
    }
}
```
    As you can see here, the logic to check if number is even or odd is repeating.

    Instead, you can write a function that takes a number as input, checks if it's even or odd, and prints the result. And then call that function for each number you want to check.

 ```java
public class Main {
    public static void checkEvenOdd(int num) {
        if (num % 2 == 0) {
            System.out.println(num + " is even");
        } else {
            System.out.println(num + " is odd");
        }
    }

    public static void main(String[] args) {
        checkEvenOdd(5);
        checkEvenOdd(6);
    }
}
```
In this way you only write the logic once and use it multiple times, avoiding repetition of code.



</Callout>

## ⭐ Class


<div className= "mt-3"></div>
<div className="cardTexture5">
    <h1 style={{padding: "8px"}} className = "mb-8 text-center font-bold text-transparent sm:text-4xl text-[25px] tex bg-clip-text bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-sky-700 via-cyan-500 to-neutral-300" align="middle">

        What is Class ?
    </h1>
    <h11 className="textStyle1 " >

        <p align="center">
            <img style={{ position: "relative" ,opacity: 1 ,borderRadius: "10px" ,overflow: "hidden" , marginTop:"20px" , marginBottom: "20px"}}
                 src="https://media.giphy.com/media/zYqEs9YpduDa8gn6pR/giphy.gif"
                 width="450"/>
        </p>

        Let's say you have a collection of toy cars. Each toy car is different - some are red, some are blue, some are small, some are big, etc. But they are all toy cars.

        In object-oriented programming (OOP), you can use a class to represent the concept of a toy car. The class would define what a toy car is (it's a small model car that can be played with) and what it can do (it can be rolled along the ground, it can be painted different colors, etc.).

        The class would be like a blueprint for making toy cars. You can use the blueprint to make as many toy cars as you want, each one with its own set of characteristics (color, size, etc.). Each toy car is an object of the "ToyCar" class.

        So, in real life, a class is like a blueprint for making something. And an object is an instance of that blueprint.
        <div className="mt-8"></div>
        <h12 className ="font-bold text-2xl sm:text-4xl align-middle ml-8">Then what is Class 😥❓</h12>
        <div className="mb-8"></div>

        <h12 className ="font-bold text-red-500 dark:text-red-200"> A class is a blueprint for creating objects. </h12>

        <Callout type="warning" emoji="ℹ️">
            - Classes do not consume memory. They are just a blueprint for creating objects.
            - Objects inherit methods and variables from classes.
            - It is a logical entity.
        </Callout>



    </h11>
</div>


## ⭐ Object


<div className= "mt-3"></div>
<div className="cardTexture5">
    <h1 style={{padding: "8px"}} className = "mb-8 text-center font-bold text-transparent sm:text-4xl text-[25px] tex bg-clip-text bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-sky-700 via-cyan-500 to-neutral-300" align="middle">

        What is Object ?
    </h1>
    <h11 className="textStyle1 " >

        <p align="center">
            <img style={{ position: "relative" ,opacity: 1 ,borderRadius: "10px" ,overflow: "hidden" , marginTop:"20px" , marginBottom: "20px"}}
                 src="https://media.giphy.com/media/zgSIp2b2kuMq5lRKBU/giphy.gif"
                 width="450"/>
        </p>
        Imagine you're at a store that sells shoes. Each shoe in the store is an object of the "Shoe" class. Each shoe has its own unique characteristics like brand, color, size, and price.

        The class "Shoe" defines what a shoe is and what it can do. For example, the class may have a method for trying on a shoe or a method for buying a shoe. Each shoe object can use these methods to perform the corresponding actions.

        So, each shoe in the store is an object of the "Shoe" class. And each object has its own set of characteristics and actions. And each shoe can be bought by different customers.

        <div className="mt-8"></div>
        <h12 className ="font-bold text-2xl sm:text-4xl align-middle ml-8">Then what is Object 😥❓</h12>
        <div className="mb-8"></div>

        <h12 className ="font-bold text-red-500 dark:text-red-200"> A Object is an instance of a class. </h12>

        <Callout type="warning" emoji="ℹ️">
            When a class is defined, no memory is allocated but when it is instantiated (i.e. an object is created) memory is allocated. Every object has some address and it occupies some space in memory.
        </Callout>



    </h11>
</div>



## 📕 Hands Written Notes


<div className= "mt-3"></div>
<div className="cardTexture5">
    <h1 style={{padding: "8px"}} className = "mb-8 text-center font-bold text-transparent sm:text-4xl text-[25px] tex bg-clip-text bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-sky-700 via-cyan-500 to-neutral-300" align="middle">

     Hands Written Notes
    </h1>
    <h11 className="textStyle1 " >


        <PhotoProvider  toolbarRender={({ rotate, onRotate }) => {return  <Icon9 onClick={() => onRotate(rotate + 90)} />}}>
            <PhotoView className=" mt-6 border-sky-200 border-opacity-20 imageBorderNormal" src="https://github.com/Subham-Maity/Object-Oriented-Programming-For-Beginners/raw/main/01.%20Introduction%20to%20Object%20Oriented%20Programming/ss.png" alt="example">
                <img className=" mt-6 border-sky-200  border-opacity-20 imageBorderNormal" src="https://github.com/Subham-Maity/Object-Oriented-Programming-For-Beginners/raw/main/01.%20Introduction%20to%20Object%20Oriented%20Programming/ss.png" alt="example" />
            </PhotoView>
        </PhotoProvider>


    </h11>
</div>
