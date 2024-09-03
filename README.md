```cpp
info.hpp
#ifndef INFO_HPP
#define INFO_HPP

#include <string>

void printInfo();
void printInterests();
void printContact();
void printGoodbye();
void printEmployment();
void printPortfolio();
void printTechnicalSkills();
void printOther();
void printBioLoop();

#endif // INFO_H

info.cpp
#include <iostream>
#include "info.h"

void printInfo()
{
    std::cout << "Hi, I am Rafal Leszczynski" << std::endl;
    std::cout << "I am 37 years old." << std::endl;
    std::cout << "I am currently learning C++ at:" << std::endl;
    std::cout << "https://coders.school/" << std::endl;
    std::cout << "I am also learning to work with Unreal Engine and Blender." << std::endl;
    std::cout << "In 2023, I participated in a hackathon in Krakow." << std::endl;
    std::cout << "I am looking to collaborate on joint projects." << std::endl;
    std::cout << std::endl;
}

void printInterests()
{
    std::cout << "My interests include playing musical instruments," << std::endl;
    std::cout << "solving problems, solving puzzles like the Rubik's Cube," << std::endl;
    std::cout << "Einstein's riddles, and similar challenges." << std::endl;
    std::cout << "I also enjoy playing games and I'm interested in game development, including asset creation," << std::endl;
    std::cout << "node handling, and other aspects of game design and development." << std::endl;
    std::cout << "I also enjoy learning algorithms." << std::endl;
    std::cout << std::endl;
}

void printContact()
{
    std::cout << "Email: rafal_leszczynski87@wp.pl" << std::endl;
    std::cout << "Phone: 603477475" << std::endl;
    std::cout << "Facebook: https://www.facebook.com/RafalLeszczynskiFB" << std::endl;
    std::cout << "Replit: https://replit.com/@RafaLeszczynski" << std::endl;
    std::cout << std::endl;
}

void printGoodbye()
{
    std::cout << "Thank you for visiting my GitHub bio card! See you next time :)" << std::endl;
    std::cout << std::endl;
}

void printEmployment()
{
    std::cout << "I am currently looking for employment as a junior C++ programmer." << std::endl;
    std::cout << "I am open to remote, hybrid, and stationary positions," << std::endl;
    std::cout << "but prefer to work in the Lower Silesia region." << std::endl;
    std::cout << "If you are interested in my profile, please feel free to contact me!" << std::endl;
    std::cout << std::endl;
}

void printPortfolio()
{
    std::cout << "I have worked on several projects, including..." << std::endl;
    // Tutaj możesz dodać listę swoich projektów
    std::cout << std::endl;
}

void printTechnicalSkills()
{
    std::cout << "My technical skills include:" << std::endl;
    std::cout << "- C++ with object-oriented programming and STL" << std::endl;
    std::cout << "- Visual Studio" << std::endl;
    std::cout << "- Unreal Engine" << std::endl;
    std::cout << "- Git" << std::endl;
    std::cout << "- Algorithms" << std::endl;
    std::cout << std::endl;

    std::cout << "I have experience with:" << std::endl;
    std::cout << "- Scrum methodology" << std::endl;
    std::cout << "- SOLID principles" << std::endl;
    std::cout << "- STUPID principles" << std::endl;
    std::cout << std::endl;

    std::cout << "Languages:" << std::endl;
    std::cout << "- English (good comprehension and reading skills," << std::endl;
    std::cout << "with room for improvement in speaking)" << std::endl;
    std::cout << std::endl;

    std::cout << "I am interested in learning/working with:" << std::endl;
    std::cout << "- Linux" << std::endl;
    std::cout << "- QT" << std::endl;
    std::cout << "- C#" << std::endl;
    std::cout << "- Blender" << std::endl;
    std::cout << "- Software Testing" << std::endl;
    std::cout << "- Cmake" << std::endl;
    std::cout << "- Debugging" << std::endl;
    std::cout << std::endl;
}

void printOther()
{
    std::cout << "Other information..." << std::endl;
    // Tutaj możesz dodać dodatkowe informacje, które uważasz za ważne
    std::cout << std::endl;
}

void printBioLoop()
{
    while (true)
    {
        std::cout << "Choose a category:" << std::endl;
        std::cout << "1. Personal Info" << std::endl;
        std::cout << "2. Interests" << std::endl;
        std::cout << "3. Contact" << std::endl;
        std::cout << "4. Employment" << std::endl;
        std::cout << "5. Portfolio Projects" << std::endl;
        std::cout << "6. Technical Skills" << std::endl;
        std::cout << "7. Other" << std::endl;
        std::cout << "8. Exit" << std::endl;
        std::cout << std::endl;

        int choice;
        std::cin >> choice;

        switch (choice)
        {
            case 1:
                printInfo();
                break;
            case 2:
                printInterests();
                break;
            case 3:
                printContact();
                break;
            case 4:
                printEmployment();
                break;
            case 5:
                printPortfolio();
                break;
            case 6:
                printTechnicalSkills();
                break;
            case 7:
                printOther();
                break;
            case 8:
                printGoodbye();
                return;
            default:
                std::cout << "Invalid choice. Please try again." << std::endl;
                std::cout << std::endl;
                break;
        }
    }
}

main.cpp
#include <iostream>
#include "info.hpp"

int main()
{
    std::cout << "Welcome to my GitHub bio card!" << std::endl;
    std::cout << "Would you like to learn more about me?" << std::endl;
    std::cout << std::endl;

    printBioLoop();

    return 0;
}

```
