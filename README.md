# leedcode-121.-best-time-to-buy-and-sell-stock
leedcode 121. best time to buy and sell stock solution

class Solution {
    public int maxProfit(int[] prices) {
        int minPrice=Integer.MAX_VALUE;
        int maxProfit=0;

        for(int i=0;i<prices.length;i++){
            if(prices[i]<minPrice){
                minPrice=prices[i];
                
            
        }
        else{
            int profit=prices[i]-minPrice;
            if(profit>maxProfit){
                maxProfit=profit;
            }
        }
        }
        
      return maxProfit;
        
    }
}
