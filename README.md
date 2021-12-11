# perfect-square-or-not

package myProjects;

import java.util.Scanner;

public class PerfectSquare {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		Scanner sc = new Scanner(System.in);
		System.out.println("enter a number");
		int n = sc.nextInt();
		int count_of_factor = 0;
		
		for (int i=1; i <= n; i++) {
			if(n % i == 0) {
				count_of_factor = count_of_factor + 1;
			}
		}
		if (count_of_factor % 2 != 0) {
			System.out.println("is perfect square");
		}
		else {
			System.out.println("is not perfect square");
		}
	}

}
