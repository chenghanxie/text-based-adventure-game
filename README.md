# Pseudocode
"""This is a text based adventure game that user will enter inputs until the game is over. A game can be over. either you survived or you are killed. Your goal is to survive until the end. Choose wisely."""

while True: 
  initial_game_choice = input(""" You find yourself in the middle of nowhere after you wake up from sleep, you realized you are trapped in the area. 
  You need to try your best, use everything around you to get out and find rescue. First, you find some cold weapons like axe, sword lying around. 
  You can choose 1. Bring all the cold weapons, and logging for fire. Or 2. Don't bother to carry anything, want to get out as soon as possible. (Choose 1 or 2) """)
  #This is the initial game choice, both choices lead to completely different story

  if initial_game_choice == "1":
    print(" ")
    first_choice = input(""" Not a bad choice! You have the tools to logging for fire now! 
    Do you want to 1. Start logging right away. Or 2. Trying to find a place to settle for sleep. (Choose 1 or 2) """)
    #This is the first choice after the initial choice
    
    if first_choice == "1":
      print(" ")
      second_choice = input(""" Ok this is definitely reasonable, You got some logs of wood and set on fire succesfully. And you even manage to cook some food! 
      Now you don't have to worry about hunger anymore. Now you desperately want to get out this place. 
      Do you want to 1. Patiently wait a few days. Or 2. Decide to try your luck and walk around for help. (Choose 1 or 2) """)
      #This is the second choice after the initial choice
      
      if second_choice == "1":
        print(" ")
        third_choice = input(""" Wow, you choose to patiently wait, that's an interesting decision. But your decision is actually right because there are a lot of bears hanging around you. 
        Few days later, you see some hikers and you are so excited. They ask you to team up, do you want to 1. Remind them the bears and patiently wait again. Or 2. Team up yay. (Choose 1 or 2) """)
        #This is the third choice after the initial choice
        
        if third_choice == "1":
          print("As expected, those hikers got attacked by the bears and all dead. But congrats to you because you finally wait until the rescue team come. Now you can get out this evil place!!!")
          break;
          #This means you've won the game, this choice is right, also breaks the loop. 

        elif third_choice == "2":
          print("You choose to team up with those hikers. You totally forget the bears and as expected, all of you got attacked by it and died.")
          break;
          #This means you've failed(got killed), this choice is not ideal, also breaks the loop

      elif second_choice == "2":
        print("Sadly, when you walk out for help, you find yourself surronded by bears, and you died from bear attack.") 
        break;
        #This means you've failed(got killed), this choice is not ideal, also breaks the loop    

    elif first_choice == "2":
      print("Ok now you settle down and sleep. You died inside your dreams because there is no fire and you are frozen to death.")
      break;
      #This means you've failed(got killed), this choice is not ideal, also breaks the loop

  elif initial_game_choice == "2":
    print(" ")
    first_choice1 = input(""" Ok so you don't want to do anything, you just want to get out. So you walk for 6 hours staright and now you have to make a choice again. 
    You can choose 1. the grassland on your left. Or 2. the woods on your right. (Choose 1 or 2) """)
    #This is the first choice after initial choice

    if first_choice1 == "1":
      print(" ")
      second_choice1 = input(""" Not bad! You manage to find an abandoned car on the grassland. 
      Do you want to 1. fix the car. Or 2. Nah I will use my bare feet to walk out. (Choose 1 or 2) """)
      #This is the second choice after initial choice

      if second_choice1 == "1":
        print("Nice. You successfully fixed the car, and you drive out from the grassland and get rescued. What a miracle!!!")
        break;
        #This means you've won the game, this choice is right, also breaks the loop. 

      elif second_choice1 == "2":
        print("Ok so you choose your bare feet as your transportation tool. Unfortunately this is grassland so you got attacked by cheetahs while you are walking.")
        break;
        #This means you've failed(got killed), this choice is not ideal, also breaks the loop

    elif first_choice1 == "2":
      print("So you choose the woods. After 30 minutes of walking, you are getting attacked from multiple animals and inspects, and soon you feel nausea and died inside this dangerous woods place.") 
      break;
      #This means you've failed(got killed), this choice is not ideal, also breaks the loop

"""The end"""

