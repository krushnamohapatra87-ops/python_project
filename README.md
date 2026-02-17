# python_project
python pratices problems 
my python_projects
day_name=input("enter a day: ")
expense_new=int(input("enter a expense: "))
protein_new=int(input("enter a protein: "))


data_items = {
  "day1":{"expense":140,"protein":110},

  "day2":{"expense":150,"protein":150},
  "day3":{"expense":100,"protein":100},
  "day4":{"expense":expense_new,"protein":protein_new}
}
total_kharcha=0

for day, stats in data_items.items():
    
    total_kharcha += stats["expense"]

    if stats["protein"]>=100:
        print(f"{day}: protein Goal met")
    else:
        print(f"{day}: protein Goal not met")
print(f"\nTOtal expense:{total_kharcha} INR")
for items in data_items.keys():
    print(items)
for value in data_items.values():
    print(value)
if "protein" in data_items:
    print("protein diya he")

