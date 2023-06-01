import datetime
import time
import sys

def sunday_pay():
    print('the cost of parking all day is £2.50')
    total = float(input("enter cash: "))
    while total < 2.50:
        addition = float(input('enter cash: '))
        total = total + addition
    else:
        print('you have entered a total of',total)
        if total > 2.50:
            change = total - 2.50
            print('your change is',change)
            print('you are now allowed to parking for the whole day')
def mon_to_sat_pay():
    print("up to 1 hr: £1 ")
    print("up to 2 hr: £2.10 ")
    print("up to 3 hr: £3.10 ")
    print("up to 4 hr: £4.30 ")
    print("up to 6 hr: £6.40 ")
    print("6+ hrs upt to 24hrs: £9.20")
    print("after 9 am shoppers up to 5 hrs: £3")

    daystotal = float(input("enter the amount you'd like to pay to park: "))
    Done = False

    while daystotal < 1 and Done == False:
        addmore = float(input('enter cash: '))
        daystotal = daystotal + addmore
        question = ("press enter if thats all you'd like to put in, if not press any other key")
        if question == '':
            Done == True
    if daystotal < 2.10 and daystotal >= 1:
      print('you can park up to one hour')
      userchange = daystotal - 1
      print('your change is £',userchange)
    elif daystotal >= 2.10 and daystotal < 3.10:
        print('you can park up to 2 hours')
        userchange = daystotal - 2.10
        print('your change is £',userchange)
    elif daystotal >= 3.10 and daystotal < 4.30:
        print('you can park up to 3 hours')
        userchange = daystotal - 3.10
        print('your change is £',userchange)
    elif daystotal >= 4.30 and daystotal < 6.40:
        print('you can park up to 4 hours')
        userchange = daystotal - 4.30
        print('your change is £',userchange)
    elif daystotal >= 6.40 and  daystotal < 9.20:
        print('you can park for up to 6 hours')
        userchange = daystotal - 6.40
        print('yoour change is £',userchange)
    elif daystotal >= 9.20:
        print('you can park for up to 24 hours')


total = 0


#finding current date using datetime function and storing in the'today' variable
today = datetime.datetime.now()
# we can now refer to the variable 'today' which carries all the information we need if we wanted to pull info about the current date.
#I used the strftime method to convert to a string.
#%A is a format for the weekdays full name which i used individually because im only interested in the day of the week.The following can also been used to show details about the present time (%B =month, %d =day of month, %Y= year XXXX)
day = today.strftime('%A')
#printing the day
print('Day:', day)


#finding current time
current_time = time.strftime("%H:%M:%S")
print('time:',current_time)


the_hour = datetime.datetime.now()
#used this to convert the current hour from a string to integer by multiplying by ten.
format_int = the_hour.hour*10

print('welcome to town hall car park')
print('accepted cash: 0.10, 0.20, 0.50, 1, 2, 5, 10')

if day == 'Sunday':
    while format_int < 90 and format_int > 0:
#90 represents 9 AM. I multiplied it by ten to convert to integer earlier in 'format_int' variable.
        print('the car park is closed')
        print('Sundays opening times are 9AM to midnight')
        exit()
    else:
     sunday_pay()
else:
    while format_int < 70 and format_int > 0:
#70 represents 7 AM. I multiplied it by ten to convert to integer earlier in 'format_int' variable.
        print('the car park is closed')
        print('Monday-Saturday opening times are from 7AM to midnight')
        (exit)
    else:
     mon_to_sat_pay()

