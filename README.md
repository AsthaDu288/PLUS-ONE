# PLUS-ONE
#A non-empty array of digits representing a non-negative integer, increment one to the integer.
class Solution {
    public int[] plusOne(int[] digits) {
        int n=digits.length;
        for(int i=digits.length-1;i>=0;i--){
            if(digits[i] < 9){
                digits[i]++;
               return digits;
            }
            else{
                 digits[i]=0;
                 
            }
        }
       
        int[] arr = new int[n+1];
        arr[0]=1;
        return arr;
    }
}
