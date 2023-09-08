# aiml
data=[3,23,34,5,7,8,9,21,56,0,14,11,12,22,43,32,89,98,6,45,1]
data.sort()
print(data)
elem=int(input("enter the element"))
def binary_search(data,elem):
    low=0
    high=len(data)-1    
    while low<=high:        
        middle=(low+high)//2        
        if data[middle]==elem:
            print(f"the searching element is{elem} present at intex value {middle}in dataset")
            break        
        elif data[middle]>elem:
            high=middle-1        
        else:
            low=middle+1
    if data[middle]!=elem:
        print(f" the searching element is {elem}  not present in the dataset")
        return
    
