# Ada-Curriculum - beggining journey into coding

import random

# step 2 list of student names
names = ["ROSIE MARTINEZ", "JOE LIU", "SALLY SUE", "BOB JOHNSON", "DELIA AGHO"]

# step 3 list of student ids randomly generated
ids = []
for i in range(5):
    ids.append(random.randint(111111, 999999))

# step 4 list of emails using student first letter name + last name + ids
emails = []
i = 0
for name in names:
  [first, last] = name.split(" ")
  emails.append(first[0]+last+str(ids[i])[-3:]+"@adadev.org")

# step 5 print each student accounts information
for i in range(5):
    print(f"name: {names[i]}")
    print(f"id: {ids[i]}")
    print(f"email: {emails[i]}\n")
