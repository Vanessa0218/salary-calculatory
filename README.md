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
	System.out.println( hours * rate);
	//calculating monthly pay
	System.out.println((hours * rate) * 52 /12);
	//annual pay
	System.out.println( monthly * 12);
	//calculating income tax, EI, CPP
	System.out.println(annual / 15);
	System.out.println(annual / 1.62);
	System.out.println(annual / 5.10);
	System.out.println(annual - tax - EI - CPP);
	}//main end
}//class end
