
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <stdlib.h>
#define NUM 30


void main()
{
	//קולט 30 משתנים
	printf("enter %d grades\n",NUM);
	int grades[NUM];
	int MA = 0;
	int NA = 0;
	float max = 0, min = 0, sum;
	int index;
	for (index = 0; index < NUM; index++)
	{
		scanf("%d\n", &grades[index]);
		if (grades[index] < 0)
		{
			index = NUM;
			printf("Error! please write positive numbers!");
		}
		


		//maximum
		if (max < grades[index])
			max = grades[index];
		if (max = grades[index])
			MA++;
		// minimum
		if (min < grades[index])
			min = grades[index];
		if (min = grades[index])
			NA++;
	}
printf("minimum is %f\n", min);
		printf("amount of times shown: %d\n", MA);
		printf("maximum is %f\n", max);
		printf("amount of times shown: %d\n", NA);
	system("pause");
}

