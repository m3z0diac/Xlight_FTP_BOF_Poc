# Xlight_FTP_BOF_Poc


### Discovered by:
```Yehia Elghaly```
### Discription:
Xlight FTP 3.9.3.1 'Access Control List' Buffer Overflow (PoC)

### Steps to reproduce:
 1. - Download and Xlight FTP
 2. - Run ```python3 -c "print('A'*600)"``` and copy those characters
 3. - Open Xlight FTP 3.9.3.1
 4. - "File and Directory - Access Control List - Setup - Added users list directories
 5. - Go to Specify file or directory name applied or Specify username applied to or Specify groupname applied
 6. - Go to Setup -> added -> Enter new Item -  Paste the characters 
 7  - Crashed
 
 ### Note:
 you can not overwrite the eip register or any other register, so don't wast your time creating the shellcode for execute a command on the server
