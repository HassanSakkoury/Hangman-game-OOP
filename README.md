# Hangman-game-OOP
class hangman:
    def __init__ (self):
        self.lives = 3
        self.word1 = 'movie'
        self.word2 = 'ball'
        self.word3 = 'food'
        
    def check_answer (self):
        
        print('you have 3 lives only')
        
        answer1 = input('enter the secret word: ')
        if answer1 == self.word1 or answer1 == self.word2 or answer1 == self.word3:
            print('Wow..! right answer.')
        else:
            self.lives -= 1
            print('wrong answer you have 2 lives left')     
            
        answer2 = input('enter your the word: ')
        if answer2 == self.word1 or answer2 == self.word2 or answer2 == self.word3:
            print('Wow..! right answer.')
        else:
            self.lives -= 1
            if self.lives == 0:
                print('Game Over')
            else:
                if self.lives == 2: 
                    print('wrong answer you have 2 lives left')
                else:
                    print('you have 1 life left')
                    
        answer3 = input('enter the secret word: ')           
        if answer3 == self.word1 or answer3 == self.word2 or answer3 == self.word3:
            print('Wow..! right answer.')
            
        else:
            self.lives -= 1
            if self.lives == 0:
                print('Game Over')
            else:
                if self.lives == 2:
                    print('wrong answer you have 2 lives left')
                else:
                    self.lives == 1
                    print('wrong you have 1 life left.')
                    
        answer4 = input('enter the secret word: ')
        if answer4 == self.word1 or answer4 == self.word2 or answer4 == self.word3:
            print('Wow..! right answer.')
        else:
            self.lives -= 1
            if self.lives == 0:
                print('Game Over')
                
            else:
                if self.lives == 2:
                    print('wrong answer you have 2 lives left')
                else:
                    self.lives == 1
                    print('wrong you have 1 life left.')
                 
        answer5 = input('enter your secret word: ')
        if answer5 == self.word1 or answer5 == self.word2 or answer5 == self.word3:
            print('Wow..! right answer.')
        else:
            if self.lives == 2:
                print('wrong answer you have 2 lives left')
            else:
                self.lives == 1
                print('Game Over')
