import java.util.Scanner;

public class anagramstring {
	public static void main(String args[]){
		
		Scanner sys=new Scanner (System.in);
		
		System.out.println("Enter The String to be Check for Anagram.");
		
		System.out.print("\nEnter The First String : ");
		String s1=sys.next();
		
		System.out.print("Enter The Second String : ");
		String s2=sys.next();
		
		int length,count=0,flag=0,temp=0;;
		
		if(s1.length()==s2.length()){
			length=s1.length();
			
			for(int i=0;i<length;i++){
				count=0;
				for(int j=0;j<length;j++){
					if(s1.charAt(i)==s2.charAt(j)){
						count=1;
						break;
					}
				}
				if(count==0){					
					flag=1;
					break;
				}
			}			
			
			if(flag==1){
				System.out.println("\nThe Input Strings are not Anagram.");
			}
			else
				System.out.println("\nThe Input Strings are Anagram.");
			
		}
		else
			System.out.println("\nThe Input Strings are not Anagram.");
		
		
	}
}
