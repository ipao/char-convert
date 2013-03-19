#char-convert

Bookmarklet for convert wrong type language from English to Thai.

##Prepare

1. Turn on bookmark or favorite toolbar. (Instruction for [Firefox](http://support.mozilla.org/en-US/kb/bookmarks-toolbar-display-favorite-websites#os=win7&browser=fx19), [Google Chrome](http://support.google.com/chrome/bin/answer.py?hl=en&answer=95745), [Internet Explorer](http://windows.microsoft.com/en-us/windows-vista/show-or-hide-the-favorites-bar-in-internet-explorer-8))
2. Left Click on toolbar that you has just turn on to add new bookmark.
3. Type "char-convert" for the name of new bookmark.
4. Copy this code to new bookmark url/location.

```
javascript:(function(){var en=["1","2","3","4","5","6","7","8","9","0","-","=","\\","!","@","#","$","%","^","&","*","(",")","_","+","|","q","w","e","r","t","y","u","i","o","p","[","]","Q","W","E","R","T","Y","U","I","O","P","{","}","a","s","d","f","g","h","j","k","l",";","'","A","S","D","F","G","H","J","K","L",":","\"","z","x","c","v","b","n","m",",",".","/","Z","X","C","V","B","N","M","<",">","?"],th=["ๅ","/","-","ภ","ถ","ุ","ึ","ค","ต","จ","ข","ช","ฃ","+","๑","๒","๓","๔","ู","฿","๕","๖","๗","๘","๙","ฅ","ๆ","ไ","ำ","พ","ะ","ั","ี","ร","น","ย","บ","ล","๐","\"","ฎ","ฑ","ธ","ํ","๊","ณ","ฯ","ญ","ฐ",",","ฟ","ห","ก","ด","เ","้","่","า","ส","ว","ง","ฤ","ฆ","ฏ","โ","ฌ","็","๋","ษ","ศ","ซ",".","ผ","ป","แ","อ","ิ","ื","ท","ม","ใ","ฝ","(",")","ฉ","ฮ","ฺ","์","?","ฒ","ฬ","ฦ"],result='',strInput=window.getSelection().toString();if(strInput=='')strInput=prompt("Insert text for convert to right Thai characters.");if(strInput != ''){for (i=0;i<strInput.length;i++){if(strInput.charCodeAt(i)==10)result+='\n';else{for(j=0;j<92;j++){if(strInput.charAt(i)==en[j]){result+=th[j];break;}}if(j==92)result+=strInput.charAt(i);}}alert(result);}})();
```
Click save or add this new bookmarklet.


##How to use

1. Drag the wrong words that you want to changed.
2. Click "char-convert" bookmarklet on bookmark or favorite toolbar.
3. If you not selected words. It will show popup the input field and you may type the words manually.
4. The characters that convert to Thai successful will show in the new popup.


## Changed Log

### 1.0
* Can convert wrong English character to Thai by selection words. 
