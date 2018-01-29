#compilar 
Assignment 1
#include <iostream>
#include <string.h>
using namespace std;


int main()
{
	int i, count=0;
char word[100];
cout<<"enter a sentence:"<<endl;

 cin.get(word,100);
 int len = strlen(word);
for(i=0; i<len;i++)
{
	if(word[i]==' ')
	count++;
}
cout<<"the number of space in the sentence is : "<<" "<<count<<endl;
int k=0;
for(int j=0; j<len; j++)
     if(word[j] != ' '){
        word[k] = word[j];
        k++;
     }
    word[k] = '\0';

cout<<"Remove space: "<<word<<endl;

return 0;
}

