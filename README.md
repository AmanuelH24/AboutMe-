- [About Me](https://github.com/AmanuelH24/AboutMe-#about-me)
- [Hobbies](https://github.com/AmanuelH24/AboutMe-#hobbies)
- [Life After Collage](https://github.com/AmanuelH24/AboutMe-#life-after-collage)
- [Block of Code](https://github.com/AmanuelH24/AboutMe-#block-of-code-i-wrote-using-c)

## About Me 
My Name is Amanuel Hailemariam.I am from kansas city, Mssouri. 

I am a student at [**University Of Missouri**](https://missouri.edu/) Columbia, 
studying *Information Technology*.

![Image of university of Missouri](https://www.thesecu.com/wp-content/uploads/2015/06/05-Campus_Aerial-2017-960x540.jpg "University of Missouri Campus")



## Hobbies 
When I have free time I really enjoy playing soccer and music. 

Some of my favorite music instruments to play are

- Guitar. 
- Piano/Keyboard. 
- I also just picked up the bass guitar and I really enjoy it. 
- Here is a link to a video I recorded for an assigment of me playing some guitar cordes [Guitar Video](https://vimeo.com/747376459)

![Image of Music Insterments](https://previews.123rf.com/images/osaba/osaba1606/osaba160600635/58043424-selective-focus-microphone-and-blur-musical-equipment-guitar-bass-drum-piano-background-.jpg)




## Life After Collage 

After I am done with collage I am planning on working in **Web Developmet, Cyber Security or some type of SoftWare Development**. 

I also always liked airplanes so I might get my private pilot license.

Also once I figure out what I really like doing with *Information Technology* I might go back to school to expand on my degree. 

![](https://www.seriun.co.uk/wp-content/uploads/2022/03/Seriun-IT-The-real-cost-of-not-investing-in-Cyber-Security.jpg)





## Block of Code I wrote using C#

This is one of the first project I wrote when I started learning C#

using System;
using System.Collections.Generic;
namespace GradeConverter
{
    class Program
    {
        static void Main(string[] args)

        {  
           float total_score = 0;
           Console.WriteLine("Please enter your First Name ");
           String FirstName= Console.ReadLine();

           Console.WriteLine("Please enter your Last Name");
           String LastName= Console.ReadLine();

           Console.WriteLine("Hello {0}, {1} Welcome to the Grade Converter!", FirstName , LastName);
           bool get_grade = true;

             while(get_grade) 
             {
                List<float> grades = new List<float>(); 
                Console.WriteLine("Enter the number of grades you need to convert: "); 
                int num = int.Parse(Console.ReadLine());
                float userval;
                
                for(int x = 0; x<num; x++)
                {
                    userval = getGrade();
                     grades.Add(userval);
                }
                foreach(float grade in grades)
                {
                    Console.WriteLine($"A score of {grade} is {getLetterGrade(grade)} grade"); 
                    total_score += grade;
                }
                    float score_avg = 0;
                    score_avg = total_score/num;
                    Console.WriteLine($"Averge grade: {score_avg}, which is {getLetterGrade(score_avg)} ");
                    Console.WriteLine("\nDo you want to convert more grade? (y/n): ");
                    string do_again = Console.ReadLine();
                        if(do_again != "y" && do_again != "Y")
                        {
                            get_grade = false;
                        }
            }       
        }

        static float getGrade ()
        {
                        float userValue;
                        do
                        {
                            try
                            {
                                Console.WriteLine("please enter a grade");
                                userValue = float.Parse(Console.ReadLine());
                                if(userValue >= 100)
                                {
                                    Console.WriteLine("Invalid number! Please try again!");
                                    continue;
                                }
                                else
                                {
                                    break;
                                }
                            }
                            catch(Exception)
                            {
                                Console.WriteLine("There was an error. Please try again");
                                userValue = float.Parse(Console.ReadLine());
                            }
                            return userValue;
                        }while(userValue < 0 );
                        return userValue; 
        }
        static string getLetterGrade(float uservalue)
        {
            {
             if( uservalue >= 90)
             {
             
                return "A";
             }
             else if(uservalue >= 80 )
             {
                 return "B";
             }
             else if(uservalue >= 70)
             {
                 return "C";
             }
             else if(uservalue >= 60)
             {
                 return "D";
             }
             else 
             {
                 return "F";
             }
            }
        }
    }   
}


I hope this gave you a little bit of an idea on who I am. 

***THANK YOU FOR READING***

