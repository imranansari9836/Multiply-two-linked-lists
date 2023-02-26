
class GfG{
  /*You are required to complete this method */
   public long multiplyTwoLists(Node l1,Node l2){
          //add code here.
          long num1=0;
          long num2=0;
          long N=1000000007;
          while(l1!=null || l2!=null)
          {
              if(l1!=null)
              {
                  num1=((num1)*10)%N +l1.data;//32
                  l1=l1.next;//0
              }
              if(l2!=null)
              {
                  num2=((num2)*10)%N +l2.data;//1000
                  l2=l2.next;//0
              }
          }
          return ((num1%N)*(num2%N))%N;
          
   }
}
