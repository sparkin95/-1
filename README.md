# -1
简单网站爬虫
import urllib
import os
def main():
    url=input("输入一个网站：").strip()
    infile=urlib.urlopen(url)
    s=infile.read().decode()

    counts=countLetters(s.lower())

    for i in range(len(counts)):
        if counts[i]!=0:
            print(chr(ord('a')+i)+"appears"+str(counts[i])+("time"if counts[i]==a else"times"))
def countLetters(s):
    counts=26*[0]
    for ch in s:
         if ch.isapha():
             counts[ord(ch)-ord('a')]+=1
    return counts
main()
os.system("pause")

            
