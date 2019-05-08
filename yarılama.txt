#include <stdio.h>
#include <stdlib.h>
#include <math.h>

#define f(x) (x*x -2*x - 2)

int main()
{
	double a = 0, b = 3, p;
	int k = 0;
	double e = 0.001;

	do {

		k++;
		p = (a + b) / 2;
		printf("a=%f      b=%f     p=%f    f(p)=%f \n ", a, b, p, f(p));

		if (f(p) > 0) {
			b = p;
		}
		else {
			a = p;
		}


	} while ((fabs(f(p))) > e);


	printf("root =%f   and iteration =%d \n", p, k);
	return 0;
}