# c-scanf-2
CSDN搜寻到对scanf(“%*[^\n]%*c”)解释
//#include <stdio.h>
//int main()
//{
//
//int att;
//char fee[100];
//printf("enter the number:\n");
//scanf("%d",&att);
//printf("enter yes or no:\n:");
//rewind(stdin);  //解决方案 
//scanf("%s",fee);
//printf("%d %s",att,fee);
//
//
//return 0;
//}


#include <stdio.h>
int main()
{

int att;
char fee[100];
printf("enter the number:\n");
scanf("%d",&att);
printf("enter yes or no:\n:");
scanf("%*[^\n]%*");  //第二种解决方案 
scanf("%s",fee);
printf("%d %s",att,fee);


return 0;
}
