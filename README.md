# java-programs-using-if-else
package com.Day4;

import java.util.Scanner;

public class main {
	public static void main(String[] args) {

		try (Scanner subjects = new Scanner(System.in)) {
			System.out.print("Enter subject1 marks : ");
			int sub1 = subjects.nextInt();

			System.out.print("Enter subject2 marks : ");
			int sub2 = subjects.nextInt();

			System.out.print("Enter subject3 marks : ");
			int sub3 = subjects.nextInt();

			System.out.print("Enter subject4 marks : ");
			int sub4 = subjects.nextInt();

			System.out.print("Enter subject5 marks : ");
			int sub5 = subjects.nextInt();

			double totalMarks = (sub1 + sub2 + sub3 + sub4 + sub5);
			double total = (totalMarks * 100) / 500;

			if (total <= 100 && total >= 90) {
				System.out.println("Your Results : " + total + "%" + " And Your Grade is A");
			} else if (total <= 90 && total >= 80) {
				System.out.println("Your Results : " + total + "%" + " And Your Grade is B");
			} else if (total <= 80 && total >= 70) {
				System.out.println("Your Results : " + total + "%" + " And Your Grade is C");
			} else if (total <= 70 && total >= 60) {
				System.out.println("Your Results : " + total + "%" + " And Your Grade is D");
			} else {
				System.out.println("Your Results : " + total + "%" + " And Your Grade is F");
			}
		}

	}
}
