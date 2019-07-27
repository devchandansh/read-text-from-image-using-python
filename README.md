# Requirements

Python Version = 3.6.5
Pillow==6.1.0
pytesseract==0.2.7



/*
*	Normally, Tesseract on Debian GNU Linux, but there was also the need for a Windows version. 
*	That's why we are installing it on windows.
*
*	To make IT works on Windows machine
*	Making all solutions together, Just Follow the sequence.
*/


#Step-1: 
	/* Install tesseract using windows installer available at:  */
	
	https://github.com/UB-Mannheim/tesseract/wiki

#Step-2:
	/* Install pytesseract */
	
	pip install pytesseract

#Step-3:
	
	/*
	*	Set the PATH of Installed "tesseract". Set the installed Path
	*	PATH may be "C:\Program Files (x86)\Tesseract-OCR\tesseract.exe"
	*	Check the path in your machine.
	*/

	import pytesseract
	pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files (x86)\Tesseract-OCR\tesseract.exe" 

#Step-4:
	Now call "image_to_string"


