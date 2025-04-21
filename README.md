## 📜 HEAD-AND-TAIL UTILITY
CLI Tool | File Processing | Head/Tail Functionality

A lightweight command-line utility combining head/tail features
with support for both line-based and byte-count operations.

## 🚀 KEY FEATURES
✔ Dual functionality: head + tail in one tool                                            
✔ Flexible units: Count by lines (-l) or bytes (-b)                                                                    
✔ Stream support: Files or stdin input                                                        
✔ Help system: Built-in usage documentation                                                                

## ⚡ QUICK USAGE
1. First 10 lines (default)
$ ./ht -l 10 file.txt

2. Last 20 bytes
$ ./ht -t -b 20 file.txt

3. Pipe support
$ cat large.log | ./ht -l 15

4. Help menu
$ ./ht --help

## 🛠️ INSTALLATION
- Clone and build                                  
$ git clone https://github.com/yourrepo/head-tail-utility.git                                  
$ cd head-tail-utility                          
$ make                                                

## 🖥️ EXAMPLE OUTPUT
1. Help Message                                    
$ ./ht --help                                                          
usage: ./ht [--help] [-h|-t] [-b|-l number] [filename]                                                                              
Options:                                              
  --help          Show this help message                                                          
  -h              Head mode (default)                                                         
  -t              Tail mode                                                
  -b              Count by bytes (default)                                              
  -l              Count by lines                                     
  number          Units to display (default: 10)                                                          
  filename        Input file (stdin if omitted)                                                                 

2. Head Mode (Lines)
$ ./ht -l 5 sample.txt                                                                                                               
Line 1: This is                                                    
Line 2: a sample                                                              
Line 3: text file                           
Line 4: demonstrating                                   
Line 5: head output                    

3.  Tail Mode (Bytes)                                                
$ ./ht -t -b 20 sample.log                                            
�[2023] End of file                                                  

## 📌 DEFAULT BEHAVIOR                              
Mode: head (-h)                    
Unit: bytes (-b)                            
Count: 10                         
Input: stdin (if no file specified)                               

## 💡 PRO TIPS
🔧 Combine with other CLI tools via pipes                                           
📝 Use -l for log file inspection                                            
⚡ Defaults make quick checks effortless                         
📚 --help shows all options                                 
