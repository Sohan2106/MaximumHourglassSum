import java.io.*;
import java.util.*;

public class Hourglass{

  public static void main(String[] args) {
    try(Scanner input = new Scanner(System.in)){
      int arrayOfElements[][] = new int[6][6];
        ArrayList<Integer> listOfSum = new ArrayList<>();
             
        takeInput(input,arrayOfElements);
        calculateHourglassSum(arrayOfElements,listOfSum);
        printMaximumSum(listOfSum);
    }
  }
    
  private static int hourglassSum(int hgRow, int hgCol, int[][] array){
    int sum = 0;
    for(int row = hgRow; row <= hgRow+2 ; row++){
      for(int col = hgCol ; col <= hgCol+2; col++){
        if(row == hgRow+1 && (col == hgCol || col == hgCol+2)){
          continue;
        }
    
        else{
          sum += array[row][col];
        }
      }
    }
    return sum;
  }
    
  private static void takeInput(Scanner input,int[][] array){
    for(int row=0; row < 6; row++){
      for(int col=0; col < 6; col++){
        array[row][col] = input.nextInt();
      }
    }
  }
    
  private static void calculateHourglassSum(int[][] array,ArrayList listOfSum){
    int temp;
    for( int row=0; row < 4; row++){
      for( int col=0; col < 4;col++){
        temp = hourglassSum(row,col,array);       
        listOfSum.add(temp);
      }
    }
  }
    
  private static void printMaximumSum(ArrayList<Integer> listOfSum){
    int max = listOfSum.get(0);
    for(int row=1;row < listOfSum.size();row++){
      if(max < listOfSum.get(row)){
        max = listOfSum.get(row);
      }
    }
    System.out.println(max);
  } 
}
