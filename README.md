# заполнение списка new_list уникальными значения из списка nun_list

n = int(input()) #количество элементов спска
num_list = []
for i in range(n):
    num_list.append(str(input())) # заполняем список строками
new_list = []
for i in num_list:
    if i not in new_list: # если элеента старого списка нет в новом 
        new_list.append(i) #- переносим его в новый списко
print(*new_list, sep='\n')
