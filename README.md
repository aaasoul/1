# 1
4.8
#include "stdio.h"

int main(int argc, char* argv[])
{
	int  a[3][3];
    int *i,csum[3],rsum[3],sum1,sum2,cflag,j,k;
     i=&(a[0][0]);
	
	for(i[0]=1;i[0]<10;i[0]++){
		for(i[1]=1;i[1]<10;i[1]++){
			if(i[1]==i[0])
				continue;
			for(i[2]=1;i[2]<10;i[2]++){
				if(i[2]==i[0]||i[2]==i[1])
					continue;
				for(i[3]=1;i[3]<10;i[3]++){
					if(i[3]==i[0]||i[3]==i[1]||i[3]==i[2])
						continue;
					for(i[4]=1;i[4]<10;i[4]++){
						if(i[4]==i[0]||i[4]==i[1]||i[4]==i[2]||i[4]==i[3])
							continue;
						for(i[5]=1;i[5]<10;i[5]++){
							if(i[5]==i[0]||i[5]==i[1]||i[5]==i[2]||i[5]==i[3]||i[5]==i[4])
								continue;
							for(i[6]=1;i[6]<10;i[6]++){
								if(i[6]==i[0]||i[6]==i[1]||i[6]==i[2]||i[6]==i[3]||i[6]==i[4]||i[6]==i[5])
								   continue;
								for(i[7]=1;i[7]<10;i[7]++){
										if(i[7]==i[0]||i[7]==i[1]||i[7]==i[2]||i[7]==i[3]||i[7]==i[4]||i[7]==i[5]||i[7]==i[6])
								     continue;
										for(i[8]=1;i[8]<10;i[8]++){
											if(i[8]==i[0]||i[8]==i[1]||i[8]==i[2]||i[8]==i[3]||i[8]==i[4]||i[8]==i[5]||i[8]==i[6]||i[8]==i[7])
								        continue;
								        
										for (j = 0; j < 3; j++)
                                        {
                                            csum[j] = 0;
                                            rsum[j] = 0;
                                        }
                                        sum1 = 0;
                                        sum2 = 0;
                                        
                                        for (j = 0; j < 3; j++)
                                        {
                                            for (k = 0; k < 3; k++)
                                            {
                                                csum[k] += a[j][k];
                                                rsum[j] += a[j][k];
                                            }
                                            sum1 += a[j][j];
                                            sum2 += a[j][2 - j];
                                        }
                                        if (sum1 != 15|| sum2 != 15)
                                            continue;
                                            
                                            cflag=0;
                                            
                                            for (j = 0; j < 3; j++)
                                        {
                                            if (csum[j] !=15 || rsum[j] != 15)
                                            {
                                                cflag = 1;
                                                break;
                                            }
                                        }
                                        if(cflag==0)

										for(j=0;j<3;j++){
							                 for(k=0;k<3;k++){

									printf("%d",a[j][k]);
										}
									printf("\n");
								}
							printf("\n");
							}
						}
					}
				}
			}
		}
	}

								
										
				
							}
						}

					

           


 return 0;
} 
