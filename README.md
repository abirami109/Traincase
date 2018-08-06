# Traincase
import java.io.*;
import java.util.scanner;
class train 
 {
 public static void main(String[] args) 
  {
  int d,e,f;
		int s1=0,s2=0,s3=0,ch;
		int x[]={22,119,64,177,21};
		int y[]={22,111,87,193,22};
		int z[]={11,107,93,162,42};
		double t[]={6.04,9.04,12.04,15.04,19.04};
		Scanner sc=new Scanner(System.in);
   do
    {
    System.out.println("Enter choice:1.Displaying train details\n
                                     2.Finding popular train\n
                                     3.Finding least popular train\n
                                     4.Finding 6.04 is popular than 9.04 or not\n
                                     5.If 6.04 on monday is popular than 6.04 on tuesday\n
		                     6.Finding popular train by your choice\n
                                     7.Display passenger no below 50\n
                                     8.Average no of passengers on 12.04 train\n
                                     9.Average no of passengers on train of your choice\n
                                     10.Quit");
    ch=sc.nextInt();
    switch(ch)
     {
      case 0:
       System.out.println("Day \t\t Departure Time \t\t No of Passengers\t\t");
	for(int i=1;i<=5;i++)
		{
			System.out.println("Monday\t\t"+t[i]+"\t\t\t"+x[i]);
		}
	for(int i=1;i<=5;i++)
		{
			System.out.println("Tuesday\t\t"+t[i]+"\t\t\t"+y[i]);
		}
	for(int i=1;i<=5;i++)
		{
			System.out.println("Wednesday\t\t"+t[i]+"\t\t\t"+x[i]);
		}break;

      case 1:
        System.out.println("Day \t\t Departure Time \t\t No of Passengers\t\t);
        System.out.println(+x[1] "\t"  +y[1]        "\t\t" x[1]          \t\t);

      case 2:
       if(d>e && d>f)
		{
		System.out.println("The most popular train is on Monday and the time is "+t[s1]);
		}
       if(e>d && e>f)
		{
		System.out.println("The most popular train is on Tuesday and the time is "+t[s2]);
		}
       if(f>e && f>d)
		{
		System.out.println("The most popular train is on Wednesday and the time is "+t[s3]);
		}break;
      case 3:
       if(d<e && d<f)
		{
		System.out.println("The least popular train is on Monday and the time is "+t[s1]);
		}
       if(e<d && e<f)
		{
		System.out.println("The least popular train is on Tuesday and the time is "+t[s2]);
		}
       if(f<e && f<d)
		{
		System.out.println("The least popular train is on Wednesday and the time is "+t[s3]);
		}break;
      case 4:
       if((x[0]<x[1] && y[0]<y[1]) && (x[0]<x[1] && z[0]<z[1]) && (y[0]<y[1] && z[0]<z[1]))
		{
		System.out.println("The popular train time is 9.04");
		}
       else
		{
                System.out.println("The popular train time is 6.04");
                }break;
      case 5:
       for(int i=1;i<=5;i++)
		{
			if(x[i]<y[i])
			{
			s1++;
			}
		}
       if(s1>s3)
		{
                System.out.println("The popular train is on Tuesday");
                }
       else
		{
                System.out.println("The popular train is on Monday");
                }break;
       case 7:
         for(int i=0;i<5;i++)
		{
	        if(x[i]<50)
			{
			System.out.println("The train with passengers less than 50 on Monday:"+t[i]);
			}
		if(y[i]<50)
			{
			System.out.println("The train with passengers less than 50 on Tuesday:"+t[i]);
			}
		if(z[i]<50)
			{
			System.out.println("The train with passengers less than 50 on Wednesday:"+t[i]);
			}
		}break;
       case 8:
        int average;
        average=(x[2]+y[2]+z[2])/3;
        System.out.println("Average number of passengers that travelled on 12.04 train : " +average);
       case 9:
        int ch1,average;
        switch(ch1)
         {
         case 1:
             average=(x[0]+y[0]+z[0])/3;
             System.out.println("Average number of passengers that travelled on 6.04 train : " +average);
         case 2:
             average=(x[0]+y[0]+z[0])/3;
             System.out.println("Average number of passengers that travelled on 9.04 train : " +average);
         case 3:
             average=(x[0]+y[0]+z[0])/3;
             System.out.println("Average number of passengers that travelled on 12.04 train : " +average);
         case 4:
             average=(x[0]+y[0]+z[0])/3;
             System.out.println("Average number of passengers that travelled on 15.04 train : " +average);
         case 5:
             average=(x[0]+y[0]+z[0])/3;
             System.out.println("Average number of passengers that travelled on 19.04 train : " +average);
         }break;
        case 10:
         string quit,repeat;
         System.out.println("ch:(quit/repeat)");
         ch=sc.nextLine();
         if(ch=exit)
           {
           System.exit(0);
           }
         else
           {
           goto 1;
           }break;
         }
   while(ch!=10);
  }
 }
           
                

        
        
       
       
       
       
