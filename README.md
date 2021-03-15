# Converse-Inverse-Contrapositive-Operations
#include<iostream>
#include<string>
using namespace std;
class Operations
{
public:
	void converse()
	{
		string P, Q, Swap;
		cout << " Enter the propostions " << endl;
		cin >> P;
		cin >> Q;
		Swap = P;
		P = Q;
		Q = Swap;
		cout << "The converse is:" << P << "->" << Q << endl;
	}

	void inverse()

	{
		string P, Q;
		cout << " Enter the propostion " << endl;
		cin >> P;
		cin >> Q;
		if (P == "P" && Q == "Q")
		{
			P = "-P", Q = "-Q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}
		if (P == "-P" && Q == "Q")
		{

			P = "P", Q = "-Q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "P" && Q == "-Q")
		{

			P = "-P", Q = "Q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "-P" && Q == "-Q")
		{

			P = "P", Q = "Q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "p" && Q == "q")
		{

			P = "-p", Q = "-q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}
		if (P == "-p" && Q == "q")
		{

			P = "p", Q = "-q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}
		if (P == "p" && Q == "-q")
		{

			P = "-p", Q = "q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "-p" && Q == "-q")
		{

			P = "p", Q = "q";
			cout << "The inverse:" << P << "\t" << "->" << Q << endl;
		}
		else
		{

			cout << " Condition is invalid !!! " << endl;
		}
	}

	void contrapositive()
	{
		string P, Q, Swap;
		cout << " Enter the propostion " << endl;
		cin >> P;
		cin >> Q;
		if (P == "P" && Q == "Q")
		{
			P = "-P", Q = "-Q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}
		else if (P == "-P" && Q == "Q")
		{
			P = "P", Q = "-Q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}
		if (P == "P" && Q == "-Q")
		{

			P = "-P", Q = "Q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "-P" && Q == "-Q")
		{
			P = "P", Q = "Q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" <<"->"<< Q << endl;
		}

		if (P == "p" && Q == "q")
		{
			P = "-p", Q = "-q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "-p" && Q == "q")
		{

			P = "p", Q = "-q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}

		if (P == "p" && Q == "-q")
		{
			P = "-p", Q = "q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive:" << P << "\t" << "->" << Q << endl;
		}
		if (P == "-p" && Q == "-q")
		{
			P = "p", Q = "q";
			Swap = P;
			P = Q;
			Q = Swap;
			cout << "The contrapositive = " << P << "\t" << "->" << Q << endl;
		}
		else
		{
			cout << " Condition is invalid !!! " << endl;
		}
	}
};

int main()
{
	Operations O;
	int choice;
	do
	{
		cout << " Press 1 for Inverse " << endl;
		cout << " Press 2 for Converse " << endl;
		cout << " Press 3 for Contrapositive " << endl;
		cout << " Press 4 for exit " << endl;
		cin >> choice;
		if (choice == 1)
		{
			O.inverse();
		}
		if (choice == 2)
		{
			O.converse();
		}
		if (choice == 3)
		{
			O.contrapositive();
		}
	}
	while (choice != 4);
	system("pause");
	return 0;
}
