import java.util.Scanner;

class Add{
	static int arr[] = new int[100];
	
	static float sum=0;
	static int flag=0;
	static Scanner input = new Scanner(System.in);
	public static void addarr()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		int MAX=0;
		int MIN=999;
		System.out.println("Enter "+ n +" elements of array");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		for(int i=0;i<n;i++)
		{
			if(arr[i]>MAX)
			{
				MAX=arr[i];
			}
			if(arr[i]<MIN)
			{
				MIN=arr[i];
			}
		}
		System.out.println("Max element in array is: " +MAX+" and Minimum number in array is :"+MIN);
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.addarr();
	}
}
