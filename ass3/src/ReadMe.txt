

In this assignment we insert the meaningful text which is "This is a private key and we encrypted with your password" at the end of private key. 
After the decrypt steps we search this meaningful text in decrypted private key.

Running Steps: 
	Running steps is same at the assignment pdf.
	javac ichecker.java
	java ichecker createCert -k PriKey -c PubKeyCertificate
	java ichecker createReg -r RegFile -p Path -l LogFile -h Hash -k PriKey
	java ichecker check -r RegFile -p Path -l LogFile -h Hash -c PubKeyCertificate

Important notes:
	You do not have to add any extension for private key file or certificate file. This code using autofill for extension and check with same extension. So please just write path like:
	
	
	java ichecker createCert -k C:/users/priKey -c C:/users/certificate 
