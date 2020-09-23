<div align="center">

## A bin2dec converter


</div>

### Description

A binary to decimal converter
 
### More Info
 
A binary number

the number in decimal


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[koby\-GR](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/koby-gr.md)
**Level**          |Beginner
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |C
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/koby-gr-a-bin2dec-converter__3-6690/archive/master.zip)





### Source Code

```
/* Binary to decimal converter
 *
 *        by : koby
 *           koby@in.gr
 * If you like this code, visit my site
 *           http://www.codecraft.tk
 */
#include <stdio.h>
#include <math.h>
int main(void) {
	int dec=0, flag=0.0;
	int bin, bit;
	double exp=0.0;
	printf("Enter a binary number : ");
	scanf("%d", &bin);
	while(bin) {
		bit=bin%10;
		if(bit!=0 && bit!=1) {
			flag=1;
		}
		bin=bin/10;
		dec=dec+bit*pow(2, exp);
		exp++;
	}
	if(flag) {printf("\n+++ Not a binary number !!!\n");}
	else {printf("\n+++ Number in decimal : %d\n", dec);}
	return 0;
}
```

