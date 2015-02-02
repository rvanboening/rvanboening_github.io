Jason's Checksplitter and Dinner Party code project
``````````````````````````
class DinnerClub
  
  attr_accessor :members, :restaurant
    
  def initialize(restaurant, *members)
    @members = members
    @restaurant = restaurant
    @member_payment_history = {}
  end
`````````````````````````````

This is what is happening at the beginning of your code. 
First you declare a new class called DinnerClub. You know this is a class because: 1. it says class. 2. it is capitolized.

after that you define two attr_accessor: 
members and restaurant
  def member
    @member #this returns the instance variable member
  end
   and the same for restaurant. 
   
Then you initialize members, resaurant, and member_payment_history into instance variables. 
Member_payment_history is a hash. 
You state that you have two arguments to be filled. resturant and members. 



```````````````````````
  def new_split_amount_custom_tip(group_number, meal_cost, tip)
    check_split = CheckSplitter.new(group_number, meal_cost, tip)
    check_split.split_check_custom_tip
  end
``````````````````````````````````````````````
because your CheckSplitter is a class of its own don't you just have to call the class with the correct number of arguments in order to make it work? 

def new_split_amount_custom_tip(group_number, meal_cost, tip)
 check_split=checkSplitter.new(group_number, meal_cost, tip)
end

I'm not toally sure but maybe try it. 

Overall Good Job, just keep plugging away. 
 _
  