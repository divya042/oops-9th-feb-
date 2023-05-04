```python
Which function is used to open a file ?
what are the different modes of operating file?
explain each mode of file opening.

Ans- 
    The built-in python functions used to open a file is 'open()'
    The 'open()' function takes two parameters: The name of the file, and the mode in which you want to open the file.
    The different modes of opening a file are:
         
            1.'r'(read only) - This is the default mode.It opens the file for reading and an error is raised if the file 
            doent;
            2.'w'(write only) - this mode opens the file writing.If the file already exits, its content is truncated(i.e.
            deleted
            3.'a'(Append only) - This opens the file for writing ,but it appeds the new data to the end of the file instead of 
                                                                                                                     
            4.'b'(Binary)- This mode is used to open the file in binary mode.It can be combined with any of the modes above e.g
                                                                                                                     
            5.'x'(Exclusive creation) -This mode is similar to 'w' but it opens the file only if it doesn't already exist.
                                                                                                                     
            6.'t'(Text)- This mode is open the file in text mode.It can be combined with any of the modes above(e.g
                                                                                                                     
            
    
```


```python
2.Why close() function is used ? Why is it important to close a file?

Ans - 
      The 'close' function is used to a file that was previously opened with the 'open()' function.
    It's important to  close a file after you are done with it several reasons:
           1. Releasing system resources : when you open a file,your operating system allocates system resources (such asmemory
                    
           2.Flushing buffered data:  when you write to a file , the data is often buffered in memory before its actually written
                                                                                                                  
           3.preventing data corruption: if you don't close a file after writing to it ,there is a risk that data may become corruption
                                                                                                                  
           4.Improving program robustness:Failing to close a file can lead to unpredictable behaviour and bugs in your program
             it's good to practice to close a file after you are done.
```


```python
3.write a python program to create  a text file.write 'I want to become  data scientist' in that file . Then close the file.open

Ans -
     # open the file in write mode
    file = opEN("My_file.txt","w")
    
    #write to the file 
    file.write("I want to become a Data scientist")
    
    #close the file
    file.close()
    
    #open the file in read mode
    file = oprn ("My_file.text","r")
    content = file.read()
    
    #open the file in read mode
    file = open ("My_file.text", "r")
    content = file read()
    
    # read the content of the file
    content = file.read()
    
    #print the content of the file
    print(content)
    
    #close the file
    file.close()
    
    This code will file named 'My_file.text' in the current directory,write the specified text to it ,close the file 
    
```


```python
4.Explain the following with python code:read(),readline() and readlines().

Ans- In python 'read()' method reads the entire contents of the file and returns it as a single string.
     for example: 
          
            #open the file in read mode
            file = open("My_file.txt","r")
            
            #print the content of the file
            print(content)
            
            #close the file 
            file.close()
            
2.'readline()'- The 'readline()' methof reads a single line from a file and returns it as astring.
   
    For example:
            
            #open the file in read mode
            file = open("Myfile.txt","r")
            
            #read the first lineline of the file
            first_line = file.readline()
            
            #print the first line of the line 
            print(first_line)
            
            #close the file 
            file.close()
            
            
            
 3. 'readlines()' - The 'readlines()' method read all the lines of a file and returns them as a alist of strings
  
       For example: 
                   #open the file in read mode
                    file = open("My_file.txt","r")
                    
                    #Read all the lines of the file 
                    lines = file.readlines()
                    
                    #Print all the lines of the file
                    for lines in lines:
                        print(line)
                        
                        #close the file
                        filr.close()
                        
            


```


```python
5. Explain whythe statement is used with open().what is the advantages of using with statements and open() together.

Ans- 
     The 'with' statement is used in the 'open()' function ,you need to reminder to close the file when you are done with it,
    
    For example- 
             with open("my_file_txt","r") as file:
            content = file.read()
            print(content)
            
advantages - It eliminates that risk of forgetting to close the file ,which can result in data loss or corruption. 
             by automatically closing the file when its no longer needed , the 'with' statement ensure that the file is closed corruption
            
             In hort,using the 'wth' statement with the 'open()'function is good practice that makes your code more readable 
```


```python
6.Explain the write() and writelines() functions. Give a suitable example.
 
Ans.   
     1.'write()' - The 'write()',function writes string to a file.
    
    For example: 
                 
              #open the file in write mode
                file = open ("my_file.txt","w")
                
                #write to the file
                file.write("I want to become a Data scientist")
                
                #close the file 
                file.close()
                
     2. 'writelines()' - The 'writelines()" function write a list of string to a file .
    
    For example:
        
            #open the file in write mode 
            file = open("my_file.txt","w")
            
            #write a list of string to the file 
            lines = ["Line 1","Line 2 ","Line 3"]
            file.writelines(lines)
            
            #close the file 
            file.close()
                
```
