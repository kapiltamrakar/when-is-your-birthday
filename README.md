# when-is-your-birthday

import datetime

print("-----------------------------------")
print("      when is your birthday")
print("-----------------------------------")
print ()
user_name = input("Hey, what is your name")

print("when is your birthday {}".format(user_name))
user_year  = int(input("year-[YYYY]"))
user_month = int(input("month-[MM]"))
user_day   = int(input("day-[DD]"))

birth_date = datetime.date(user_year, user_month, user_day)

today_date = datetime.date.today()
print(today_date)

this_year_birth_date = datetime.date(today_date.year, birth_date.month, birth_date.day)
print(this_year_birth_date)
date_diff = this_year_birth_date - today_date
print(date_diff.days)

if date_diff.days < 0:
    print("hey {}, your birthday was  before {} days,hope you have enjoyed it".format(user_name, date_diff.days))
elif date_diff.days > 0:
    print("hey {}, your birthday is in {} days,hope you are looking forward for it".format(user_name, date_diff.days))
else:
    print("hey {}, topday is your birthday, wishing you a happy birthday!".format(user_name))
    



                
        
    



