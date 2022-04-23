# Demo
First time using GitHub

import random
print('ROCK, PAPER, SCISSORS')
wins = 0
losses = 0
ties = 0

while True:
    print('%s Wins, %s Losses, %s Ties' % (wins, losses, ties))
    while True: #the player's input loop.
        print('Enter your move: (r)ock, (p)aper, (s)cissors or (q)uit')
        playerMove = input()
        if playerMove == 'q':
            sys.exit() #Quit the program
        if playerMove == 'r' or playerMove == 'p' or playerMove == 's':
            break #Break out of the player input loop
        print('Type one of r, p, s, or q.')

    #Display what the player choose:
    if playerMove == 'r':
        print('ROCK versus...')
    elif playerMove == 'p':
        print('PAPER versus...')
    elif playerMove == 's':
        print('SCISSORS versus...')

    #Display what the computer chose:
    random.Number = random.randint(1,3)
    if random.Number == 1:
        computerMove = 'r'
    elif random.Number == 2:
        computerMove = 'p'
    elif random.Number == 3:
        computerMove = 's'

    #Display and record the win/loss/tie:
    if playerMove == computerMove:
        print("It's a tie!'")
        ties = ties + 1
    elif playerMove == 'r' and computerMove == 's':
        print('You win')
        wins = wins + 1
    elif playerMove == 'p' and computerMove == 'r':
        print('You win!')
        wins = wins + 1
    elif playerMove == 's' and computerMove == 'p':
        print('You win!')
        wins = wins + 1
    elif playerMove == 'r' and computerMove == 'p':
        print('You lose!')
        losses = losses + 1
    elif playerMove == 'p' and computerMove == 's':
        print('You lose!')
        looses = losses + 1
    elif playerMove == 's' and computerMove == 'r':
        print('You lose!')
        looses = losses + 1
