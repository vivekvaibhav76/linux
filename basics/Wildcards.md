<h1>Wildcards</h1>
Wildcards are symbols or special characters that represents other characters.

You can use them with any commmand such as
1. ls
2. rm
3. cp

* : matches zero or more characters

eg: *.txt, c*,c*.txt

? : matches exactly one character

eg: ?.doc, c?

[ ] : Matchs any of the characted enclosed between the brackets

eg: 
   app[ole]
   apple
   appo
   
[!] : Matches any of the characters not included between the brackets. 

eg: [!aloe]
    basket
    cone

[-] : Use hyphen to create a range between the characters.

eg: [a-c]* : Matches all the files that start with a,b or c.

    [1-3]* : Matches all the files that start with 1,2 or 3.
    

    
