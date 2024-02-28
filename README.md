# CS361-test-
CS361 test file (My first repository on GitHub)
#This is a comment.
#This is a new commit from the local server. Hello World!

"""
This document provides instructions on how to interact with the random number generator microservice. The microservice allows users to receive random numbers from their intended range n.

### Requesting Data
To request a random number, we just need to make sure that in the Txt file, there is the number n inside where n stands for the range. 

file = open('prng-service.txt', 'r+')
read_file = file.readline()
if read_file.isdigit():
    time.sleep(5)
    upperLimitNum = int(read_file)


### Receiving Data
To receive data, we read the content from that same "prng-service.txt" after 5 seconds.

randNum1 = random.randint(1, upperLimitNum)
    randNum2 = random.randint(1, upperLimitNum)
    randNum3 = random.randint(1, upperLimitNum)
    randNumTple = (randNum1, randNum2, randNum3)
    returnWord = "ok" + str(randNumTple)
    file.seek(0)
    file.truncate()
    file.write(returnWord)



"""
