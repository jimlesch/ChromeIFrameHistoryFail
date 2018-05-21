Using chrome on Windows 10: Version 66.0.3359.181 (Official Build) (64-bit) 

1. start nginx (configured to listen on 8008)
2. put a host file entry in for 127.0.0.1 chromefail
3. in chrome, navigate to localhost:8008/page.html
4. click on the hyperlink: navigate to 2
5. click on the first "back" button (inside the frame). For me, nothing happens and there is no output in developer console.  Expected: same behavior as 6.
6. click on the second "back" button (outside the frame). It navigates back one page inside the frame (as expected.)


I cannot reproduce the behavior in #5 on another windows 10 machine with the same version of chrome.

Steps I have taken:
1) reset chrome settings.
2) uninstalled and reinstalled chrome stable.
3) installed chrome beta (same problem in step 5 for me)
4) running chrome with command line switch --disable-web-security
