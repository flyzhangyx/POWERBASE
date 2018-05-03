# POWERBASE
⊙∀⊙！
package myhomework;

import java.util.Scanner;

public class homework {
//------------------------------------------------------------------
	public  static void bubble(int n[],int k)//k为控制排序方式变量，1由大到小，2由小到大
	{
		switch (k)
		{
			case 1:
				for(int i=0;i<n.length;i++)
					for(int j=i+1;j<n.length;j++)
					if(n[i]>n[j])
					{
						int temp;
						temp=n[j];
						n[j]=n[i];
						n[i]=temp;
					}
						for(int i=0;i<n.length;i++)
						System.out.print(n[i]+"\t");
						break;
			case 2:
				for(int i=0;i<n.length;i++)
					for(int j=i+1;j<n.length;j++)
					if(n[i]<n[j])
					{
						int temp;
						temp=n[j];
						n[j]=n[i];
						n[i]=temp;
					}
						for(int i=0;i<n.length;i++)
						System.out.print(n[i]+"\t");
						break;
		}
	}		
//--------------------------------------------------------------
	 public static int doublefind(int n[],int k,int s)//二分查找
	{
		int i=0,m=0,l=n.length;
		if(s==1)
		{
			do
			{
				i=(m+l)/2;
				if(n[i]<k)
					m=i;
				else if(n[i]>k)
					
