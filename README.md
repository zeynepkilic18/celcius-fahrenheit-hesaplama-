# celcius-fahrenheit-hesaplama-
celcius fahrenheit hesaplama fonksiyon ile
#include<stdio.h>
/*bir kullanici celcius cinsinden verilen bir sicaklik degerini fahrenheit ,fahrenheit cinsinden verilen bir degeride celsius cinsinden bulmak istemektir.Kullaniciya
hengi tür cevrim yapacagini soran ve buna göre cevirmeyi yapan program F/f C/c kullanarak C=5/9(F-32) */


int cel_fah(int c)
{
	return (c*9/5+32);
}

int fah_cel(int f)
{
	return ((f-32)*5/9);
}


int main(void)
{   char sec;
	int derece;
	printf("Fahrenheit--> celsius icin C/c\n");
	printf("Celsius--> fahrenheit icin F/f\n");
	printf("seciminizi giriniz");
	scanf("%c",&sec);
	if(sec=='F'|| sec=='f')
	{
		printf("celcius degerini girin:");
		scanf("%d",&derece);
		printf("fahrenheit degeri: %d",cel_fah(derece));
	}
	else if(sec=='C'|| sec=='c')
	{
		printf("fahrenheit degerini girin:");
		scanf("%d",&derece);
		printf("celcius degeri: %d",fah_cel(derece));
	}
	else 
	printf("hata");
	return 0;
}
