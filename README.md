# count-of-words-vowels-and-consonants-in-string
#problem3=count of vowels,words,consonants in string
#approach1
a=input().split()
wc=len(a)
vc=0
cc=0
v="aeiouAEIOU"
for i in a:
  for j in i:
    if j.isalpha():
      if j in v:
        vc=vc+1
      else:
        cc=cc+1
print(wc,vc,cc) 

'''
#approach2
t=int(input())
v="aeiouAEIOU"
for _ in range(t):
  s=input()
  vc=0
  cc=0
  for i in s:
    if i.isalpha():
      if i in v:
        vc=vc+1
      else:
        cc=cc+1
  a=s.split()
  wc=len(a)
  print(wc,vc,cc)
