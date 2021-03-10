# hello-world
this is my first repo
a bit about myself
an edittt
https://us04web.zoom.us/j/4190089367?pwd=UWNrdVB0a2V0L3Z4WERqK2JKWTJPQT09

#include<stdio.h>

 

void main()

{

    int bt[20],p[20],wt[20],tat[20],i,j,n,total=0,pos,temp;

    float avg_wt,avg_tat;

    printf("Enter number of process:");

    scanf("%d",&n);

 

    printf("\nEnter Burst Time:\n");

    for(i=0;i<n;i++)

    {

        printf("p%d:",i+1);

        scanf("%d",&bt[i]);

        p[i]=i+1;           

    }

 

    

    for(i=0;i<n;i++)

    {

        pos=i;

        for(j=i+1;j<n;j++)

        {

            if(bt[j]<bt[pos])

                pos=j;

        }

 

        temp=bt[i];

        bt[i]=bt[pos];

        bt[pos]=temp;

 

        temp=p[i];

        p[i]=p[pos];

        p[pos]=temp;

    }

 

    wt[0]=0;             

    

    for(i=1;i<n;i++)

    {

        wt[i]=0;

        for(j=0;j<i;j++)

            wt[i]+=bt[j];

 

        total+=wt[i];

    }

 

    avg_wt=(float)total/n;      

    total=0;

 

    printf("\nProcess\t    Burst Time    \tWaiting Time\tTurnaround Time");

    for(i=0;i<n;i++)

    {

        tat[i]=bt[i]+wt[i];     

        total+=tat[i];

        printf("\np%d\t\t  %d\t\t    %d\t\t\t%d",p[i],bt[i],wt[i],tat[i]);

    }

 

    avg_tat=(float)total/n;     

    printf("\n\nAverage Waiting Time=%f",avg_wt);

    printf("\nAverage Turnaround Time=%f\n",avg_tat);

}

https://us02web.zoom.us/j/82438187830?pwd=TWQ0RElIajlhMmZSbFFtbHZkOWFMZz09


class StringBuffer1

{

      public static void main(String[]args)

        {

              StringBuffer s=new StringBuffer("Ankit");

             s= s.append(" Mandloi");

             System.out.println(s);

           s= s.insert(2,"xyz");

           System.out.println(s);

          }

}class StringBuilder1

{

      public static void main(String[]args)

        {

              StringBuilder s=new StringBuilder("Aman");

             s= s.append(" Verma");

             System.out.println(s);

           s= s.insert(2,"xyz");

           System.out.println(s);

          }

}


https://zoom.us/j/99580187530?pwd=Qlg3ZHA4UmNzYkI3a0N0bUQ5Z0J1Zz09

