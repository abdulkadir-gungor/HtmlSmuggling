# HtmlSmuggling
&emsp; HTML smuggling is a malicious technique used by hackers to hide malware payloads in an encoded script in a specially crafted HTML attachment or web page. The malicious script decodes and deploys the payload on the targeted device when the victim opens/clicks the HTML attachment/link. The HTML smuggling technique leverages legitimate HTML5 and JavaScript features to hide malicious payloads and evade security detections.

&emsp; The HTML smuggling method is highly evasive. It could bypass standard perimeter security controls like web proxies and email gateways, which only check for suspicious attachments like EXE, DLL, ZIP, RAR, DOCX or PDF

&emsp; **1) HtmlSmuggling.py :** Embeds the selected binary file (exe, dll, docx, pdf, etc) into the Javascript file. Obfuscates Javascript functions. This makes it difficult to decode javascript functions.

&emsp; "HtmlSmuggling" attack type is an attack type affected by browser settings. In addition, EXE, DLL type files downloaded from the internet can be blocked by smartscreen. However, PDF, DOCX attacks are more successful.

![htmlsmuggling](https://user-images.githubusercontent.com/71177413/174580595-4ade6473-7d2a-4ef6-ab98-c788fbd5d3e5.JPG)
&emsp; [jpg source: From the training notes, Abdulkadir GÜNGÖR]

Using the Script
---

**[Command]**
```
>> HtmlSmuggling.py filename filepath
```
&emsp; **filename:** Browser refers to the file name to be given to the file to be downloaded. It is the file name that will be seen in the browser and the downloaded folder.

&emsp; **filepath:** The path of the file to be downloaded

**[Command Example]**
```
>> HtmlSmuggling.py MicrosoftOffice.exe c:\Users\user0\Desktop\malware.exe
>> HtmlSmuggling.py Office365.dll c:\Users\user0\Desktop\malware.dll
>> HtmlSmuggling.py application.pdf c:\Users\user0\Desktop\malware.pdf
>> HtmlSmuggling.py application.docx c:\Users\user0\Desktop\malware.docx
```


The Compiled Version of the Program Can be Downloaded from the Links Below.
---
<dl>
  <dt> "Html Smuggling"
  <dd>
  <dd> HtmlSmuggling.rar --> zip password: "gung0r_HtmlSmuggling"
  <dd> Link = https://drive.google.com/file/d/1nywAbA8fEx6lFPz5snI05KeAMz8bTUcS/view?usp=sharing
</dl>


Requirement
---
&emsp; Required library: pyinstaller

```
pip install pyinstaller
```

&emsp; "pyinstaller" will be used to make the code one piece executable

Compilation
---
&emsp; [Language : Python 3.8.5]
```
pyinstaller --onefile --icon=HtmlSmuggling.ico HtmlSmuggling.py
```

Video and Screenshots of the Vulnerability
---
&emsp; The use of the compiled version of the script is shown in the Youtube video.
It can be viewed at the link below.

**[Youtube Link]** [https://www.youtube.com/watch?v=_rQrLeDaFSU](https://www.youtube.com/watch?v=ft7rdZVFv_c)

 **[ScreenShot 1]**
![b1](https://user-images.githubusercontent.com/71177413/174581941-8bc693dd-2d0c-4fa2-b1cc-900cbcd3fc0c.png)


**[ScreenShot 2]**
![a2](https://user-images.githubusercontent.com/71177413/174581963-d49e485a-b0e8-4fb1-a56c-5e85e3d3563e.png)

**[ScreenShot 3]**
![a3](https://user-images.githubusercontent.com/71177413/174581996-5c21783d-9acd-4411-bcde-b74287128ab2.png)

**[ScreenShot 4]**
![a4](https://user-images.githubusercontent.com/71177413/174582053-c683d209-ed76-449a-9897-812fa9f99edb.png)

**[ScreenShot 4]**
![a5](https://user-images.githubusercontent.com/71177413/174582090-a9d438ac-a27a-49a0-a4d4-3eeae0e32f69.png)


Legal Warning
---
&emsp; Run your tests on virtual machines. The responsibility for illegal use belongs to the user. Shared for educational purposes.
