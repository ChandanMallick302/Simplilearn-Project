package com.simplilearn;

import java.io.File;
import java.io.IOException;
import java.util.Arrays;
import java.util.Scanner;

public class Lockedme {
	public static void main(String[] args) throws IOException {
		String filename, filename1, filename2;
		int ch1, ch, ch3;
		String path = "C:\\Users\\Hackers World\\OneDrive\\Desktop\\Manas Project File\\Locked Me\\myfiles\\";

		// Take user option from bellow mentioned menu
		Scanner sc = new Scanner(System.in);
		System.out.println("*****************************");
		System.out.println("**********Locked Me**********");
		System.out.println("*****************************");
		System.out.println("********Chandan Kumar********");
		System.out.println("**Full Stack Java Developer**");
		do {
			System.out.println("\n1. Display File (Asscending order)");
			System.out.println("2. File Operation Feature");
			System.out.println("3. Exit");
			System.out.println("Please Choose the Option");
			ch = sc.nextInt();
			switch (ch) {
			case 1:
				File file = new File(path);
				String[] str = file.list();
				Arrays.sort(str);
				for (int i = 0; i < str.length; i++) {
					filename = str[i];
					System.out.println(filename);
				}
				ch = 0;
				break;
			case 2:
				do {

					System.out.println("1. Add File");
					System.out.println("2. Delete File");
					System.out.println("3. Search File");
					System.out.println("4. Go to Main Menu");
					Scanner sc1 = new Scanner(System.in);
					ch1 = sc1.nextInt();
					switch (ch1) {
					case 1:// Add File
						System.out.println("Enter The File Name");
						filename = sc.next();
						File file1 = new File(
								"C:\\Users\\Hackers World\\OneDrive\\Desktop\\Manas Project File\\Locked Me\\myfiles\\"
										+ filename + ".txt");
						if (file1.createNewFile())
							System.out.println("File is added successfully");
						else
							System.out.println("File is already existed");
						break;
					case 2:// Delete File
						System.out.println("Enter The File Name");
						filename1 = sc.next();
						File file2 = new File(
								"C:\\Users\\Hackers World\\OneDrive\\Desktop\\Manas Project File\\Locked Me\\myfiles\\"
										+ filename1 + ".txt");
						if (file2.delete()) {
							System.out.println("File is Deleted Sucessfully");
						} else {
							System.out.println("File is not exist");
						}
						break;
					case 3:// Search File
						System.out.println("Enter The File Name");
						filename2 = sc.next();
						File file3 = new File(
								"C:\\Users\\Hackers World\\OneDrive\\Desktop\\Manas Project File\\Locked Me\\myfiles\\"
										+ filename2 + ".txt");
						if (file3.exists())
							System.out.println("File is available");
						else
							System.out.println("File is not available");
						break;
					case 4:// Go to Main menu
						System.out.println("Do you want go to main menu(y/n)");
						ch1 = sc.next().charAt(0);
						if ((ch1 == 'y') || (ch1 == 'Y'))
							ch1 = 5;
						else if ((ch1 == 'n') && (ch1 == 'N')) 
							ch1=0;
							break;
					default:
						System.out.println("Please Choose Vaild Option");
						break;
					}

					
				} while (ch1 != 5);
				break;
			}
			if (ch == 3) {
				System.out.println("Applicaion closed");
			}

		} while (ch != 3);
	}
}
