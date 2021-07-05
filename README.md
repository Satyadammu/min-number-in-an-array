# min-number-in-an-array
public class Minnumber{  
public static int getMin(int[] a, int total){  
int temp;  
for (int i = 0; i < total; i++)   
        {  
            for (int j = i + 1; j < total; j++)   
            {  
                if (a[i] > a[j])   
                {  
                    temp = a[i];  
                    a[i] = a[j];  
                    a[j] = temp;  
                }  
            }  
        }  
       return a[0];  
}  
public static void main(String args[]){  
int a[]={3,9,34,24,7,4,63};  
int b[]={43,12,56,45,58,24};  
System.out.println("Min: "+getMin(a,7));  
System.out.println("Min: "+getMin(b,6));  
}}
