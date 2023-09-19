# Zeenia-Asr
def get_names(spicy_foods):
 f1=[]
 for i in spicy_foods:
  f1=f1+ [i['name']]
 return f1

def get_spiciest_foods(spicy_foods):
 f2=[]
 for i in spicy_foods:
  if i['heat_level']>=5:
   f2=f2+[i]
 return f2

def print_spicy_foods(spicy_foods):
 for i in spicy_foods:
  a=i['name']
 b=i['cuisine']
 c=i['heat_level']
 print(a,'(',b,')','Heat Level:',('🌶')*c)
 
def get_spicy_food_by_cuisine(spicy_foods,cuisine):
 for i in spicy_foods:
  f4=i['cuisine']
 if f4==cuisine:
  print(i)
  
def print_spiciest_foods(spicy_foods):
 for i in spicy_foods:
  if i['heat_level']>5:
   a=i['name']
   b=i['cuisine']
   c=i['heat_level']
   print(a,'(',b,')','Heat Level:',('🌶')*c)
   
def get_average_heat_level(spicy_foods):
 f5=0
 for i in spicy_foods:
  f5=f5+i['heat_level']
 print('Average heat level of all spicy foods is',f5/len(spicy_foods))

def create_spicy_food(spicy_foods, spicy_food):
 print(spicy_foods+[spicy_food])
spicy_food={'name': 'Griot',
'cuisine': 'Haitian',
'heat_level': 10,}
cuisine='Thai'

def main():
 print(get_names(spicy_foods))
 print(get_spiciest_foods(spicy_foods))
 print(print_spicy_foods(spicy_foods))
 print(get_spicy_food_by_cuisine(spicy_foods, cuisine))
 print(print_spiciest_foods(spicy_foods))
 print(get_average_heat_level(spicy_foods))
 print(create_spicy_food(spicy_foods, spicy_food))
 if __name__=="__main__":
  main()
