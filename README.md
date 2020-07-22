# PythonPractical3echo 
# #Working with files
# #Open; close; read; write; append; check existence; delete; with statement
#
# # # open(filename, mode)
# # #
# # # There are four different methods (modes) for opening a file:
# # #
# # # "r" - Read - Default value. Opens a file for reading, error if the file does not exist
# # #
# # # "a" - Append - Opens a file for appending, creates the file if it does not exist [adds to the end of the file]
# # #
# # # "w" - Write - Opens a file for writing, creates the file if it does not exist [overwrites the file]
# # #
# # # "x" - Create - Creates the specified file, returns an error if the file exists
# # #
# # # In addition you can specify if the file should be handled as binary or text mode
# # #
# # # "t" - Text - Default value. Text mode
# # #
# # # "b" - Binary - Binary mode (e.g. images)
# # #Open file
# # # f = open("demofile.txt")
# # # test = open("C:/Users/user/Desktop/Natalie-python-exercises.txt")
# # #
# # # n = open("demoFile.txt")
# # # n.close()
# #
# # #
# # # #Close File
# # # f = open("C:/Users/user/Desktop/pythonTextFile.txt")
# # # print(f.read())
# # # f.close()
# # #
# # # #Read File
# # # file = open("demofile.txt", "r")
# # # print(file.read()) #size	Optional. The number of bytes to return. Default -1, which means the whole file.
# # # file.close()
# # # file = open("demoFile.txt", "r")
# # # file.close()
# #
# # #
# # # #File Append
# # # g = open("demoFile.txt", "a")
# # # g.write("This is the new stuffs!!")
# # # g.close()
# # #
# # # file = open("demoFile.txt", "a")
# # # file.write("HELLO NATZ")
# # # file.close()
# #
# # # file = open("demoFile.txt", "r")
# # # print(file.read())
# # # #opepn and read file after apending:
# # # g = open("demofile.txt", "r")
# # # print(g.read())
# #
# # # test = open("demoFile.txt", "a")
# # # test.write("hi there")
# # # test.close()
# # #
# # # test = open("demoFile.txt", "r")
# # # print(test.read())
# # #
# # #
# # # #File Write
# # # g = open("demofile.txt", "w") #[overwrites the file]
# # # g.write("this is a new doggy!!")
# # # g.close()
# # # test = open("demoFile.txt", "w")
# # # test.write("HONDA")
# # # test.close()
# # #
# # # test = open("demoFile.txt", "r")
# # # print(test.read())
# # #
# # # g = open("demofile.txt", "r")
# # # print(g.read())
# # # g.close()
# # #
# # #
# # # #Create a New File [a, w, x]
# # #
# # # # newFile = open("YadzFile.txt", "x")
# #
# # #
# #new = open("MTANotes.txt", "x")
# # # # new.close()
# # # # newWFile = open("New1File.txt", "a")
# # # # test1 = open("newfileMTA.txt", "x")
# # # # test1.close()
# # # #
# # # # test2 = open("HONDA.txt", "x")
# # # # test2 = open("HONDA.txt" "w")
# # #
# # # #====================================================================
# # # #Check existence and remove file
# # #
# # # import os
# # # print("test")
# # # # #
# # # if os.path.exists("demofile.txt"): #retuns a boolean
# # #     os.remove("demofile.txt")
# # #     print("File removed")
# # # else:
# # #     print("the file does not exist")
# #
# # # import os
# # # if os.path.exists("MTANotes.txt"):
# # #     os.remove("MTANotes.txt")
# # #     print("file has been removed")
# # # else:
# # #     print("file no longer exists")
# #
# #
# # # #
# # #
# # # #Remove folder
# # #
# # # # import os
# # # # os.rmdir("myFolder")
# # #
# # # import os
# # # os.rmdir("myFolder")
# # # print("myFolder deleted")
# # # #========================================
# # #
# # # # with statement
# # #
# # # #Eg1 - without using with statment
# # # file = open("file_path", "w")
# # # file.write("Hello Yadz!")
# # # file.close()
# # #
# # # #Eg2 - without using with statment
# # # file1 = open("file1_path", "w")
# # # try:
# # #     file.write("Hello Natalie!")
# # # finally:
# # #     file.close()
# # #
# # # # - using with statement
# # # with open("file2_path", "w") as file:
# # #     file.write("Hello Yadz!!!")
# # #
# # # with open("file2_path", "w") as file:
# # #     file.write("hello Yadz!!!")
# #
# # #===============================================
# # #Get input from user
# #
# # # print("Hello user :). What is your name?")
# # #
# # # userInputName = input()
# # #
# # # print("Welcome " + userInputName)
# #
# # #print("hello user, what is your age?")
# #
# # #userAge = input()
# #
# # #print("young at heart at age " + userAge)
# #
# # print("hello user, how old are you?")
# #
# # user = input()
# #
# # ans = int(user) * 365
# #
# # print("You have been alive for " + str(ans))
# #
# # #=================================================
# #
# # #Input and File Exercise
# #
# # print("hello please input your address")
# #
# # userAddress = input()
# #
# # print("Cool, please input your school")
# #
# # userSchool = input()
# #
# # newfile = open("userdetails.txt", "x")
# # newfile.close()
# #
# # newfile = open("userdetails.txt", "w")
# # newfile.write("The user's address is: " + userAddress + " and the user's school is: " + userSchool)
# # newfile.close()
# #
# #
# # newfile = open("userdetails.txt", "r")
# # print(newfile.read())
# # newfile.close()
#
#
#
# ##========
# #Formatting output using String Modulo operater(%)
#
# print("Diamonds : % 2d, Portal : % 5.2f" %(1, 05.333))
#
# print("Total students : %3d, Boys : %2d" %(240, 120))
#
# print("Total students : " + str(240) + ", Boys : " + str(120))
#
# print("Pearl : % 2d, Wolf : % 3.3f" %(2, 5.458689))
#
# print("total students : %3d, girls : %2d" %(240, 120))
#
# #==================
# #Formatting output using format method
#
# print('I love taking my {} for a {}!'.format('dog', 'walk'))
#
# #my dog's food is old
# #my dog's food is "old"
#
# print("my dog's food is old")
print('my {} food is {}!'.format('dog\'s', 'food'))
#
# print("my dog's food is 'old'")
# print('my dog\'s food is "old"')
#
# print('my dog\'s food is old \nmy dog\'s food is "old"')
# print('my dog\'s drive me mad in my head \n i want that cat\'s "head"')
#
# #*
# #**
# #***
# #****
# #*****
#
# print("* \n** \n*** \n**** \n*****")
#
# i = 0
# star = ""
# while i < 100:
#     star = star + "*"
#     print(star)
#     i = i + 1
#
# ###################
# # FILE HANDLING REAL-WORLD
#

import sys
import io

try:
    #open file stream
    file = open("file_name.txt", "w")
except IOError:
    print("There was an error writing to file")
    sys.exit()
print("Enter File"),
print("' When finished")
while file_text != file_finish:
    file_text = raw_input("Enter text: ")
    if file_text == file_finish:
        #close the file
        file.close()
        break
    file.write(file_text)
    file.write("\n")
file.close()
file_name = raw_input("Enter filename: ")
if len(file_name) == 0:
    print("Next time please enter something")
    sys.exit()
try:
    file = open(file_name, "r")
except IOError:
    print("There was an error reading the file")
    sys.exit();
file_text = file.read()
file.close();
print( file_text)
