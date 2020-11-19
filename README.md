# TRYAD
My first game
print('Welcome to TRYAD')


name = input('What is your name? ')
age = int(input('How old are you? '))

# How to add a comma after the name value without space?

print('Hello', name, 'you are', age, 'years old.')


if age >= 18:
    print('Your age qualifies you to play this game!')
    
    consent = input('Do you want to play? ').lower()
    
    if consent == 'yes':
        print("Let's play!")
        health = 10
        
        print('You are starting with', health, 'health.')
        
        direction = input('Which way do you want to go? .... left/right? ').lower()
        
        if direction == 'left':
            
            ans = input('Great! You follow the path and reach a lava .... Will you swim across or go around it? (across/around) ').lower()
            
            if ans == 'around':
                
                print('You went around and reach the other side of the lava')
                
            elif ans == 'across':
                
                print('You managed to swim across but the lava burnt 5 health.')
# health -=5 means health = health -5
                health -= 5
            
            ans = input('You notice a snake ahead .... Will you run or wait? ').lower()
            if ans == 'run':
                print('You escape and arrive home safely')
                print('YOU WIN!')
            else:
                print('The snake bites you and you lose 5 health')
                health -=5
                
                if health <= 0:
                    print('You now have 0 health and YOU LOSE!')
                else:
                    print('You survived, YOU WIN!')
        else:
            print('You fell down and cracked you skull...')
        
    else:
        print('See you some other time.')
elif age >= 14:
    print('Your age requires you to be supervised while playing!')
    
    consent = input('Do you want to play? ').lower()
    
    if consent == 'yes':
        ans = input('Is either of your parents present? ... yes/no? ')
        if ans == 'yes':
            print("Let's play!")
        else:
            print("Sorry, but you can't play!")
        health = 10
        
        print('You are starting with', health, 'health.')
        
        direction = input('Which way do you want to go? .... left/right? ').lower()
        
        if direction == 'left':
            
            ans = input('Great! You follow the path and reach a lava .... Will you swim across or go around it? (across/around) ').lower()
            
            if ans == 'around':
                
                print('You went around and reach the other side of the lava')
                
            elif ans == 'across':
                
                print('You managed to swim across but the lava burnt 5 health.')
# health -=5 means health = health -5
                health -= 5
            
            ans = input('You notice a snake ahead .... Will you run or wait? ').lower()
            if ans == 'run':
                print('You escape and arrive home safely')
                print('YOU WIN!')
            else:
                print('The snake bites you and you lose 5 health')
                health -=5
                
                if health <= 0:
                    print('You now have 0 health and YOU LOSE!')
                else:
                    print('You survived, YOU WIN!')
        else:
            print('You fell down and cracked you skull...')
else:
    print('Your age has restricted you from playing this game!')
