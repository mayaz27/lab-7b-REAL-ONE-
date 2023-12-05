#include <iostream>
#include <string>

using namespace std;

int calculateLetterValue(char letter)
{
	switch ((char)toupper(letter))
	{
	case 'A':
	case 'E':
	case 'I':
	case 'L':
	case 'N':
	case 'O':

	//This is a comment that explains what the code below does. 
 asfdasd
 sdaf
 sadf
 sdf
 asdf
	case 'R':
	case 'S':
	case 'T':
	case 'U':
		return 1;
		break;
	case 'D':
	case 'G':
		return 2;
		break;
	case 'B':
	case 'C':
	case 'M':
	case 'P':
		return 3;
		break;
	case 'F':
	case 'H':
	case 'V':
	case 'W':
	case 'Y':
		return 4;
		break;
	case 'K':
		return 5;
		break;
	case 'J':
	case 'X':
		return 8;
		break;
	case 'Q':
	case 'Z':
		return 10;
		break;
	default:
		break;
		return 0;
	}//end switch

} //end function def

int main()
{
	string word; 

	cout << "Enter word: " << endl; 
	

	int totalScore = 0; 

	for (int i = 0; i < word.length(); i++)
	{
		totalScore = totalScore + calculateLetterValue(word[i]); //word
	}
	
	cout << "The total value of " << word << " is: " << totalScore << endl;

}
