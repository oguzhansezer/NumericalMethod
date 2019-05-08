#include <stdio.h>
#include<stdio.h>
#include<conio.h>
#include<math.h>
#include<stdlib.h>

int main()
{
	float x[5], y[5], p, s = 1, t = 1, k = 0;

	int n = 5, i, j, d = 1;

	x[0] = 1;
	x[1] = 1.3;
	x[2] = 1.6;
	x[3] = 1.9;
	x[4] = 2.2;
	y[0] = 0.7651977;
	y[1] = 0.6200860;
	y[2] = 0.4554022;
	y[3] = 0.2818186;
	y[4] = 0.1103623;

	printf("\n\n DEGER TABLOMUZ :\n\n");
	for (i = 0; i<n; i++)
	{
		printf("%0.3f\t%0.3f", x[i], y[i]);
		printf("\n");
	}
	while (d == 1)
	{
		printf(" \n\n\n Deger giriniz ? \n\n\n");
		scanf("%f", &p);
		for (i = 0; i<n; i++)
		{
			s = 1;
			t = 1;
			for (j = 0; j<n; j++)
			{
				if (j != i)
				{
					s = s*(p - x[j]);
					t = t*(x[i] - x[j]);
				}
			}
			k = k + ((s / t)*y[i]);
		}
		printf("\n\n L: %f", k);
		printf("\n\n CIKIS YAPMAK ICIN ?\n\n DEVAM ICIN 1 GIRIN CIKIS ICIN HERHANGI BIR SAYI");
		scanf("%d", &d);
	}

	return 0;
}
