import java.io.*;
import java.util.*;

public class HuxleyCode {
  public static void main(String args[]) {
  	Scanner in = new Scanner(System.in);
		double I, A, D, P;
		String S;					//(impulso)�/((Valturamario) + (distancia/2) + (peso/3))
		
		I = in.nextDouble();
		A = in.nextDouble();
		D = in.nextDouble();
		P = in.nextDouble();
		S = in.next();
		
		if (S.equals("Sim")) {
			if (Math.pow((I+5), 3) / (Math.sqrt(A) + (D/2) + ((P+50)/3)) >= 100) 
				System.out.print("Voce consegue");
			else
				System.out.print("Isso e perda de tempo");
		}
		
		if (S.equals("Nao")) {
			if (Math.pow((I), 3) / (Math.sqrt(A) + (D/2) + (P/3)) >= 100)
				System.out.print("Voce consegue");
			else
				System.out.print("Isso e perda de tempo");
		
		}  
  }
}
