# Exercise-7


#include <iostream>
using namespace std;
int main()
{
    cout << "Please enter your height in meters to check whether you can ride or not\n";
    double h, age;
    cin >> h;
    cout << "Please enter your age to check whether you can ride or not\n";
    cin >> age;
    if (age >= 5 && h >= 0.6)
    {
        cout << "You can ride";
    }
    else if (age < 5 && h < 0.5)
    {
        cout << "Sorry you cannot ride";
    }
    else
    {
        cout << "Incorrect input";
    }
    return 0;
}
  
  
  
  #include <iostream>
using namespace std;
int main()
{
    cout << "What is the capital of France?\n";
    string capital;
    cin >> capital;
   
    if (capital == "Paris" || capital == "paris" || capital == "PARIS")
    {
        cout << "You enter the correct answer";
    }
    else 
    {
        cout << "Sorry wrong answer";
    }
    
    return 0;
}
  
  
  
      #include <iostream>
using namespace std;

int main()
{
	
	char l;
	int count1, count2; // variable for isalpha
	
	cout << "Enter a letter to check whether its a vowel or a consonant: ";
	cin >> l;
	if (l == 'a' || l == 'e' || l == 'i' || l == 'o' || l == 'u'|| l == 'A' || l == 'E' || l == 'I' || l == 'O' || l == 'U') // Checking if the entered character is a vowel
	{
		cout << "The input is a vowel." << endl;
	}
	count1 = isalpha(char(l)); // Using isalpha built-in function for alphabets
	count2 = isdigit(char(l)); // Using isdigit built-in function for digits
	if (count1 == 0 && count2 != 4) // Checking if the entered character is a special character, converting the special character into their ASCII code
	{
		cout << "The input is a special character." << endl;
	}
	else if (count1 != 2 && count2 == 4) // Checking if the entered character is a digit
	{
		cout << "The input is a digit." << endl;
	}
	else if (count1 != 0 && count2 != 4 && l != 'a' && l != 'e' && l != 'i' && l != 'o' && l != 'u' && l != 'A' && l != 'E' && l != 'I' && l != 'O' && l != 'U') // Checking if the entered character is a consonant
	{
		cout << "The input is a consonant." << endl;
	}
	else
	{
		cout << "The input is incorrect.";
			}
	return 0;
}
  
  
  
  
  
  #include <iostream>
using namespace std;

int main()
{
	
	char l;
	int count1, count2; // variable for isalpha
	
	cout << "Enter a letter to check whether its a vowel or a consonant: ";
	cin >> l;
	if (l == 'a' || l == 'e' || l == 'i' || l == 'o' || l == 'u'|| l == 'A' || l == 'E' || l == 'I' || l == 'O' || l == 'U') // Checking if the entered character is a vowel
	{
		cout << "The input is a vowel." << endl;
	}
	count1 = isalpha(char(l)); // Using isalpha built-in function for alphabets
	count2 = isdigit(char(l)); // Using isdigit built-in function for digits
	if (count1 == 0 && count2 != 4) // Checking if the entered character is a special character, converting the special character into their ASCII code
	{
		cout << "The input is a special character." << endl;
	}
	else if (count1 != 2 && count2 == 4) // Checking if the entered character is a digit
	{
		cout << "The input is a digit." << endl;
	}
	else if (count1 != 0 && count2 != 4 && l != 'a' && l != 'e' && l != 'i' && l != 'o' && l != 'u' && l != 'A' && l != 'E' && l != 'I' && l != 'O' && l != 'U') // Checking if the entered character is a consonant
	{
		cout << "The input is a consonant." << endl;
	}
	else
	{
		cout << "The input is incorrect.";
			}
	return 0;
}
  
  
  
  
  
  
  #include <iostream>
#include <exception>

using namespace std;
int main()
{

    int x;
    std::cout << "Enter the marks in number to see the grade: ";
    std::cin >> x;
    //Using the cin.fail function (when user enters alphabet instead of numbers)
    if (std::cin.fail())
    {
        std::cin.clear();
        std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
        std::cout << "Incorrect command\n: ";
    }

    else if (x > 70)
    {
        cout << "You have a A Grade";
    }
    else if (x >= 60 && x < 70)
    {
        cout << "You have a B Grade";
    }
    else if (x >= 50 && x < 60)
    {
        cout << "You have a C Grade";
    }
    else if (x > 40 && x < 50)
    {
        cout << "You have a D Grade";
    }
    else if (x == 40)
    {
        cout << "You have a JUST PASSED Grade";
    }
    else if (x < 40)
    {
        cout << "You have a Fail Grade";
    }
    else
    {
        cout << "Wrong input";
    }
}
  
  
  
  
  
  
  #include <iostream>
using namespace std;

int main()
{
   cout << "Enter the marks from 1-100 to see the grade, 0 input is not accepted\n";
   double m;
   cin >> m;
   if (m>70)
   {
  cout << "You have a A Grade";
   }
   else if (m >= 60 && m < 70)
   {
  cout << "You have a B Grade";
   }
   else if (m >= 50 && m < 60)
   {
  cout << "You have a C Grade";
   }
   else if (m>40 && m<50)
   {
  cout << "You have a D Grade";
   }
   else if (m == 40 )
   {
  cout << "You have a JUST PASSED Grade";
   }
   else if(m<40 && m!=0)
   {
  cout << "You have a Fail Grade";
   }
   else 
   {
  cout << "Wrong input";
   }
}a
  
  
  
  
  
  #include<iostream>
#include<string>
using namespace std;
int main()
{
	bool musician;
	string reply;
	string instrument;
	cout << "Do you play any musical instrument? \n type 'y' for yes \n and 'n' for no \n ";
	cin >> reply;
	if (reply == "y" || reply == "Y")
	{
		musician = true;
		if (musician == true)
		{
			cout << "What kind of insturment you can play \n type d if you're a drummer \n type g if you're a guitarist\n type o for other\n" << endl;
			cin >> instrument;
			if (instrument == "g" || instrument == "G")
			{
				cout << "That's great! I really needed a guitarist." << endl;
			}
			else if (instrument == "d" || instrument == "D")
			{
				cout << "That's great! I really needed a drummer." << endl;
			}
			else if(instrument =="o" || instrument == "O")
			{
				cout << "Ah I see, actually I'm looking for guitarist or a drummer.\n Let me know if you someone who plays them\n Thank you :)" << endl;
			}
			else
			{
				cout << "Incorrect input" << endl;
			}

		}
	}
		else if (reply == "N" || reply == "n")
		{
			musician = false;
			cout << "Oh! so you don't know how to play any instrument\n it's alright, let me know if you know someone who does \n Thanks" << endl;
		}
		else
		{

			cout << "Incorrect input" << endl;
		}

	
		return 0;
	}
  
  
  
  
  
  
  
  
  
  
  #include<iostream>
using namespace std;
int main()
{
	int t, m;
	cout << "Until what time your friend will come? (Enter the time in minutes)\n";
	cin >> t;
	if (t >= 15)
	{
		cout << "Your friend will take more or equal to 15 minutes to come,\n enter the money amount to see if you can drink something";
		cin >> m;
		if (m > 5)
		{
			cout << "You have more than 5 AED, now you will buy a drink and wait for him" << endl;
		}
		else
		{
			cout << "You don't have enough money,\n Let's just walk around";
		}
	}
	else
	{
		cout << "Your friend will be here within 15 minutes, \n so you're just going to wait for him." << endl;
	}
	return 0;
}
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  #include<iostream>
using namespace std;
int main()
{

	int mag;
	std::cout << "Enter the enter the mangitude of the earthquake in numbers: ";
	std::cin >> mag;
	//Using the cin.fail function (when user enters alphabet instead of numbers)
	if (std::cin.fail())
	{
		std::cin.clear();
		std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
		std::cout << "Incorrect command\n: ";
	}
	
	else if (mag < 2.0 && mag >0) {
		cout << " earthquake is considered to be a micro earthquake.";
	}
	else if (mag >= 2.0 && mag < 3)
	{
		cout << mag << " earthquake is considered to be a very minor earthquake.";
	}
	else if (mag >= 3.0 && mag < 4)
	{
		cout << mag << " earthquake is considered to be a minor earthquake.";
	}
	else if (mag >= 4.0 && mag < 5.0)
	{
		cout << mag << " earthquake is considered to be a light earthquake.";
	}
	else if (mag >= 5.0 && mag < 6.0)
	{
		cout << mag << " earthquake is considered to be a moderate earthquake." << endl;
	}
	else if (mag >= 6.0 && mag < 7)
	{
		cout << mag << " earthquake is considered to be a strong earthquake." << endl;
	}
	else if (mag >= 7.0 && mag < 8)
	{
		cout << mag << " earthquake is considered to be a major earthquake." << endl;
	}
	else if (mag >= 8.0 && mag <= 10)
	{
		cout << mag << " earthquake is considered to be a great earthquake." << endl;
	}
	else if (mag > 10.0)
	{
		cout << mag << " earthquake is considered to be a meteoric earthquake." << endl;
	}

	else {
		cout << "You entered an invalid value" << endl;
	}
	return 0;

}
  
  
  
  
  
  
  
  
  #include<iostream>
using namespace std;
int main()
{
	double mag;
	cout << "please enter the mangitude of the earthquake in numbers 0 input is not accepted : ";
	cin >> mag;

	

		if (mag < 2.0 && mag >0) {
			cout << " earthquake is considered to be a micro earthquake.";
		}
		else if (mag >= 2.0 && mag < 3)
		{
			cout << mag << " earthquake is considered to be a very minor earthquake.";
		}
		else if (mag >= 3.0 && mag < 4)
		{
			cout << mag << " earthquake is considered to be a minor earthquake.";
		}
		else if (mag >= 4.0 && mag < 5.0)
		{
			cout << mag << " earthquake is considered to be a light earthquake.";
		}
		else if (mag >= 5.0 && mag < 6.0)
		{
			cout << mag << " earthquake is considered to be a moderate earthquake." << endl;
		}
		else if (mag >= 6.0 && mag < 7)
		{
			cout << mag << " earthquake is considered to be a strong earthquake." << endl;
		}
		else if (mag >= 7.0 && mag < 8)
		{
			cout << mag << " earthquake is considered to be a major earthquake." << endl;
		}
		else if (mag >= 8.0 && mag <= 10)
		{
			cout << mag << " earthquake is considered to be a great earthquake." << endl;
		}
		else if (mag > 10.0)
		{
			cout << mag << " earthquake is considered to be a meteoric earthquake." << endl;
		}
	
		else {
			cout << "You entered an invalid value" << endl;
		}
		return 0;
		}
  
  
  
  
  
  
