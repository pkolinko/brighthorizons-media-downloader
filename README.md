# tadpoles-media-downloader
Hack method to download all of your media from tadpoles.com and brighthorizons

***ORIGINAL AUTHOR TADPOLES.COM INSTRUCTIONS, PLEASE SEE MODIFIED BRIGHT HORIZONS INSTRUCTIONS BELOW THE ORIGINAL***

Quick script I wrote to download all pictures and videos out of tadpoles. To use, do the following:

1.) Copy the following string of text:

javascript:var js = document.createElement('script');js.src = 'https://jwally.github.io/tadpoles-media-downloader/index.js';document.querySelectorAll('head')[0].appendChild(js)

2.) Open google chrome (might work with other browsers, but not really tested)

3.) Log into tadpoles

4.) In the address bar, type the word "javascript" followed by a colon (:) like this:

javascript:

5.) Paste the text you copied earlier so your address bar now looks like this:

javascript:var js = document.createElement('script');js.src = '//bit.ly/2lKFacH';document.querySelectorAll('head')[0].appendChild(js)

6.) Hit ENTER

7.) When the website asks for permission to download multiple files, click "YES". These are your pictures and videos its trying to download.

This sounds *WAY* more complicated than it really is.
Just watch the [video](https://www.youtube.com/watch?v=c54Zx0Dx_A4)
, and if you get lost please feel free to contact me.

***MODIFIED INSTRUCTIONS FOR USE WITH BRIGHT HORIZONS***

How To: 
Note: Instructions modified for BrightHorizons MyBrightDay
 
1.) Use google chrome

2.) Log into https://familyinfocenter.brighthorizons.com or similar website

3.) The pictures are not actually stored at https://familyinfocenter.brighthorizons.com , but rather
at https://mybrightday.brighthorizons.com , so switch your view from familyinfocenter to mybrightday
as described in the next few steps: 

4.) Open "Dev Tools" in chrome
    *Windows: ctrl+shift+c
    *Mac: Command+Option+C
    *nix: ???

5.) From familyinfocenter click on one of the photos of your children to see a larger photo of your child pop up within familyinfocenter website.
    Use "Dev Tools" "Elements" tab to locate the full URL of this photo. You can search for HTML tag that starts with <img class = 
    it will have a source, src = "/remote/v1 ... " etc..
    If you don't do the steps described here, you will get a CORS error.

6.) In Dev Tools, right click on the URL and copy link address. Open a new Chrome tab and copy paste the link into the address bar. 
    You should now see the large photo of your child by itself, not embedded into the familyinfocenter frame. 
    Double check that the address bar starts with https://mybrightday.brighthorizons.com
 
7.) Paste this script in Dev Tools console

8.) Hit "Enter"
