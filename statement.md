using System;

public class Counter
{
	private int counterValue = 0;

	public void CountUp()
	{
		counterValue++;
	}

	public void CountDown()
	{
		counterValue--;
	}

	public int GetCounterValue()
	{
		return counterValue;
	}
}
   
class ExecuteEncapsulation {
	static void Main(string[] args) {
        var c = new Counter();
        Console.WriteLine(c.GetCounterValue()); //Expected 0
        c.CountUp(); // value wil be increased to: 1
        c.CountUp(); // value wil be increased to: 2
        Console.WriteLine(c.GetCounterValue()); //Expected 2
        c.CountDown(); // value wil be decreased to: 1
        Console.WriteLine(c.GetCounterValue()); //Expected 1
   }
}
