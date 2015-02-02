Holy cow. This is brilliant. 1. You make this a class of it's own. Great idea, because you can simply call the class and find the answer. I am confusued about why this is a def initalize method. Maybe you just simplified it down to this point and it may be a little beyond me so far.

I can see that your rules matrix refers to the array key of the win string. 0 = "Rock Crushes Scissors." In the next instance variable you reference play's 1 move vs. players two move with arrays inside of hashes to determine what the output should be. 

````````````````````````````````
class RPSRules
  
  include Shared_Rules_Methods
  
  # Private (Automagical): #initialize
  # Initializes a hash within a hash that says who wins within the context for rock paper scissors and
  #   what string to use when printing winner.
  #     To use, see compare_results that accesses the hash position and spits out the array position
  #     of the winner assuming the array is: [player1, player2]
  #
  # State Changes:
  # @win_strings
  # @rules_matrix
  
  def initialize
    @win_strings = ["Rock Crushes Scissors", "Paper Covers Rock", "Scissors Cut Paper", "This Round Was A Tie"]
    @rules_matrix = {"Rock"     => {"Rock" => [nil, @win_strings[3]], "Paper" => [1, @win_strings[1]], "Scissors" => [0, @win_strings[0]]},
                     "Paper"    => {"Rock" => [0, @win_strings[1]], "Paper" => [nil, @win_strings[3]], "Scissors" => [1, @win_strings[2]]},
                     "Scissors" => {"Rock" => [1, @win_strings[0]], "Paper" => [0, @win_strings[2]], "Scissors" => [nil, @win_strings[3]]}}
  end
  ``````````````````````````````````````````
  
I really enjoyed how you outputted your information to a .txt file. I think that helps conclude the program and makes it very easy to follow. 
  
  