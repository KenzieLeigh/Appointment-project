# Appointment-project
package demo;

import java.util.Scanner;

public class Client {

	public static void main(String[] args) {
		
		Scanner scannerOne = new Scanner(System.in);
		String name = "";
		
		while(name.isBlank()) {
			System.out.print("Enter your name: ");
			name = scannerOne.nextLine();
		}
		System.out.println("Welcome "+name);
		
		Scanner scanner2 = new Scanner(System.in);
		String phone = "";

		while(phone.isBlank()) {
			System.out.print("Enter your phone number: ");
			phone = scanner2.nextLine();
		}
		System.out.println("Please Review Services");
	Service.OtherMethod(args);	
	System.out.println("Thank you " + name);
	System.out.println("We will call " + phone + "if we have any further questions");
	
	}

	}
  package demo;
import java.util.*;
import demo.Client;

public class Service {

	public static void OtherMethod(String[] args) {
		// TODO Auto-generated method stub

		ArrayList<String> fullgroomList = new ArrayList<>();
		fullgroomList.add("Bath");
		fullgroomList.add("Fluff Dry");
		fullgroomList.add("Nails Cliped");
		fullgroomList.add("Ears Cleaned");
		fullgroomList.add("Brush out - no dematting");
		fullgroomList.add("Haircut and Style");
		
		ArrayList<String> tidyList = new ArrayList();
		tidyList.add("Bath");
		tidyList.add("Blow Dry");
		tidyList.add("Nails Clipped");
		tidyList.add("Ears Cleaned");
		tidyList.add("Brush out - no dematting");
		tidyList.add("Face, Feet, and Sanitary trim");
		
		ArrayList<String> bathList = new ArrayList();
		bathList.add("Bath");
		bathList.add("Blow Dry");
		bathList.add("Nails Clipped");
		bathList.add("Ears Cleaned");
		
		System.out.println("Full Grooms Include:" + fullgroomList);
		System.out.println("Tidy Up Includes: " + tidyList);
		System.out.println("Bath Only Includes: " + bathList);	
		System.out.println(" ");
		
		Scanner scanner5 = new Scanner(System.in);
		String service = "";
		
		while(service.isBlank()) {
			System.out.print("Choose a Service ");
			service = scanner5.nextLine();
		}
		System.out.println("You Chose "+service);
		
		Scanner scanner6 = new Scanner(System.in);
		String day = "";

		while(day.isBlank()) {
			System.out.print("Choose a date and time: Format mm/dd time");
			day = scanner6.nextLine();
		}

		System.out.println("You scheduled a: " + service);
		System.out.println("for " + day);
	}

}
