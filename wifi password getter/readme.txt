Explanation: Get Wifi Passwords with python
In order to get wifi passwords, we are going to use the subprocess module of Python which makes it easy to check the connected wifi passwords by allowing us to run (cmd)command prompt commands inside our program. We have two netsh commands using them we can easily see wifi passwords.

Logic is very simple, we will run cmd commands to check wifi passwords inside our program with the help of the subprocess module as mentioned above.

The two cmd commands to check connected wifi passwords are as follows:

# netsh wlan show profile
# netsh wlan show profile PROFILE-NAME key=clear


The first command is used to show the profiles of the connected wifi while 2nd is used to show the password of the wifi which you want to know.

Run cmd commands for wifi passwords in python
As mentioned earlier, we are going to use the subprocess module to run cmd commands in our python program. We will use a method from the subprocess module called check_output to run both cmd commands.

Stepwise flow of code
The main intention behind this section is that if you have a good knowledge of python then you’ll be able to make this get wifi passwords with python program on your own without looking our source code. So, the steps of implementation are as follows:

Step1: Import subprocess module.

Step2: Run the 1st cmd command using subprocess.check_output method and store the profiles data in a variable.

Step3: Convert the profile data into a list.

Step4: Iterate over the list and run the second command to check the passwords.

Step5: Store the paswords and print