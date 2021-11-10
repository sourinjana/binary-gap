# binary-gap

# you can write to stdout for debugging purposes, e.g.
# print("this is a debug message")

def solution(N):
    # write your code in Python 3.6
    value="{0:b}".format(N)
    maxgap=0
    accu=0
    for i in value:
        if i=='0':
            accu +=1

            
        elif i=='1':

            if accu>maxgap:
                maxgap=accu
            accu=0    
            b=0
    return maxgap
