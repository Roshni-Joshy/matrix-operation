# matrix-operation
//addition and multiplication of two matrices


public class Matrices
{
	public static void main(String[] args) {
		int a[][]={{1,3,4},{2,4,3},{3,4,5}};
		int b[][]={{1,3,4},{2,4,3},{1,2,4}};
		int c[][]=new int[3][3];
		int j,i,k;
		//matrix addition
		for(i=0;i<3;i++){
		    for(j=0;j<3;j++){
		        c[i][j]=a[i][j]+b[i][j];
		    }
		}
		//print resultant matrix
		System.out.println("Resultant of addition of two matrices:");
		for(i=0;i<3;i++){
		    System.out.println("");
		    for(j=0;j<3;j++){
		        System.out.print(c[i][j]);
		    }
		}   
		//multiplication of two matrices 
		for(i=0;i<3;i++){
		    for(j=0;j<3;j++){
		        c[i][j]=0;
		        for(k=0;k<3;k++){
		        c[i][j]=a[i][k]+b[k][j]+c[i][j];
		       }
		   }
		}
		//print resultant matrix
		System.out.println("Resultant of product of two matrices:");
		for(i=0;i<3;i++){
		    System.out.println("");
		    for(j=0;j<3;j++){
		        System.out.print(c[i][j]);
		    }
		}   
	
	}
}

