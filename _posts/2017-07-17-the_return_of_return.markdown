---
layout: post
title:  "The Return of `Return`"
date:   2017-07-17 20:03:24 +0000
---


When I first started coding, I didn't realize that it was frowned upon to use `return`. I was still very new to coding and often wasn't positive what the return value would automatically be so I used `return` all the time as a fail safe to ensure the correct result was returned. After starting Flatiron, I quickly realized that was a mistake and thankfully have been able to kick the bad habit to the curb. I didn't realize when I was initially using it that using `return` stops the program from continuing inside that method and reports the return value. 

As you can see below, I completed that excercise prior to beginning Flatiron and I have included three completely unneccessary returns. The program functions exactly the same if every instance of `return` was simply deleted. There are many other ways I could clean up the code below but 


```
def divisible_by_three(i)
  if i % 3 == 0 
    return true 
  end
end 

def divisible_by_five(i)
  if i % 5 == 0 
    return true 
  end
end 
  
def crazy_nums(n)
  arr = []
  i = 1 
  while i < n
 if divisible_by_five(i) == true && divisible_by_three(i) != true 
   arr = arr << i 
 end 
  if divisible_by_three(i) == true &&  divisible_by_five(i) != true
   arr = arr << i 
 end 
  i = i + 1 
  end 
return arr
end 
```

After getting accustomed to not using it, I found no way around it in my latest coding lab - the TicTacToe with AI lab. I finally now understand why `return` exists because there are situations where it is absolutely necessary to use. For example, I wanted the program to iterate through an array of winning combinations, compare those to the current board, and use that information to decide if there is a winning move available and then to return that winning move. The code I used is shown below:
```
def win_move(board)
    Players::Computer::WIN_COMBINATIONS.each do |win_combination|
      win_index_1 = win_combination[0]
      win_index_2 = win_combination[1]
      win_index_3 = win_combination[2]

      position_1 = board.cells[win_index_1]
      position_2 = board.cells[win_index_2]
      position_3 = board.cells[win_index_3]

      if position_1 == self.token && position_2 == " " && position_3 == self.token
        return "#{win_index_2 + 1}"
      elsif position_1 == " " && position_2 == self.token && position_3 == self.token
        return"#{win_index_1 + 1}"
      elsif position_1 == self.token && position_2 == self.token && position_3 == " "
        return "#{win_index_3 + 1}"
      else
        nil
      end
    end
    return nil
  end
	```
	

As you can see, `return` has returned to my code. I initally wrote the same program without using `return` but kept getting errors that an array was the output of the computer's move. I realized that because the if statement was nested inside an each enumerable, the program didn't stop when it found a winning move. It kept cycling through and then returned the original array, which was completely not helpful.

Once I added `return`, the computers started playing more as I expected them to but still missed some winning moves. After using pry and running through a few tests, I realized that I had included the `return nil` in the wrong spot.  Originally, I had `return nil` after the else statement. This meant that if the first win combination tested wasn't the one with a potential winning move, no other combinations would be tested because the #win_move method would return nil.   Finally I found the right spot for the `return nil`. Without it, the method would simply return the array of winning combinations if there was not a winning move detected.  

This is one of the dilemmas of using if/then statements inside of an enumerable. The overall method is going to return the value of the array, not the result of the if/then statement unless you use `return`.
