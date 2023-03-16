def main():
# Assignment 3-2
- It must start with the alphabet character ( ‘a~z’, ‘A~z’) 
--  isalpha() ; to check the alphabet or not
- The email string length is greater than 5 and less than 30
- use the len() function from String
- It must include the letter ‘@’
- It must include at least one ‘.’ after ‘@’

##################################################
    # Comlete your code here
  email = input('Enter your string')
  flag = True
  if not email[0].isalpha():
      flag = False
  lenemail = len(email)
  if lenemail <= 5 or lenemail >= 30:
      flag = False
  if email.find('@') == -1:
      flag = False
  else:
      atidx = email.find('@')
  if email[atidx+1:].find('.') == -1:
      flag = False
  print (flag)
if __name__ == '__main__':
    main()
    
