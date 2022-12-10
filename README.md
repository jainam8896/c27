# c27#include<iostream.h>

#include<conio.h>

#include<fstream.h>

void main()

{

	clrscr();

	ifstream fi;

	ofstream fo;

	char ch;

	fo.open("Input.txt");

	fo<<"Dharmil";

	fo.close();

	fi.open("Input.txt");

	fo.open("Output.txt");

	while(fi.eof()==0)

	{

		fi>>ch;

		fo<<ch;

	}

	fi.close();

	fo.close();

	cout<<"File Cpied"<<endl;

	fi.open("Output.txt");

	while(fi.eof()==0)

	{

		fi>>ch;

		cout<<ch;

	}

	getch();

}
