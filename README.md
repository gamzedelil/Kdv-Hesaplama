# Kdv-Hesaplama

import java.util.Scanner;

public class KdvHesaplama {

	public static void main(String[] args) {
		double tutar, kdvOran = 0.18 , kdvTutar, kdvliTutar;
		Scanner inp = new Scanner(System.in);
		
	System.out.print(" Tutari girin:");
	tutar = inp.nextDouble();
	
	kdvOran = (tutar > 1000) ? 0.8 : 0.18;
    kdvTutar = tutar * kdvOran;
    kdvliTutar = tutar + kdvTutar;
	
kdvTutar = tutar * kdvOran;
kdvliTutar = tutar + kdvTutar;

System.out.println("KDV'siz Tutar" + tutar);

System.out.println("KDV Orani:" + kdvOran);

System.out.println("KDV Tutari:" + kdvTutar);

System.out.println("KDV'li Tutar:" +kdvliTutar);

System.out.println(kdvliTutar);
	
	}

}
