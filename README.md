/*
Name: Vanessa Mahood
Course: ICS 3U
Teacher: Mrs. McCaffery
Task: Salary Calculator 

Description: Calculates your weekly/monthly/annual salary. Also calculates your
Income tex, EI, and CPP. 
*/
public class SalaryCalculater 
{
	public static void main (String[] args)
	{
		//declared variables 
	double hours = 30;
	double rate = 10.75;
	double monthly = hours * rate;
	double annual = monthly * 12;
	double tax = annual / 15;
	double EI = annual / 1.62;
	double CPP = 5.10;
	//calculating weekly pay
	System.out.println("Your weekly pay: \n$"+(hours * rate));
	//calculating monthly pay
	System.out.println("Your monthly pay: \n$"+((hours * rate) * 52 /12));
	//annual pay
	System.out.println("Your annual pay: \n$"+(monthly * 12));
	//calculating income tax, EI, CPP
	System.out.println("Your annual pay income tax deductions: \n$"+(annual / 15));
	System.out.println("Your annual pay EI deductions: \n$"+(annual / 1.62));
	System.out.println("Your annual pay CPP deductions: \n$"+(annual / 5.10));
	//annual with deductions
	System.out.println("Your annual pay with all deductions; \n$"+(annual - tax - EI - CPP));
	}//main end
}//class end
