# kissanime_anticaptcha
Learns and solves captchas on kissanime.ru  
Download at https://greasyfork.org/en/scripts/36720-kissanime-anti-captcha

kissanime captcha passer.js is a tampermonkey script that memorizes all the captchas you solve on kissanime.ru. As you solve captchas it should slowly learn almost every captcha the site has to offer (there are only about 150 unique captcha images, each of which have an average of 3 words associated with them).

If you get a captcha wrong you are (like usual) redirected to the incorrect captchas page. This page now contains a box which shows the most recent automatic captcha solves. If one of the adjectives associated with one of the images is wrong, simply click on the adjective and it will no longer be associated with the image. 
On the incorrect captchas page there is also a link which you can click at the bottom that displays every image in your database and the image's associated adjectives

__NOTE:__ for the script to work you must click the captcha images in the correct order. For example, if the captcha text says "arm, phone and lion, pink" you must click on the image of the phone followed by the image of the lion. In an attempt to force this the script automatically hides the 2nd pair of adjectives until the first image is clicked, *however,* because the script is only injected after the page fully loads, both pairs of adjectives are usually visible before the 2nd pair is hidden.

__NOTE 2:__ Without an adblocker the script might not work properly since clicking captcha images sometimes redirects you to the advertiser's page
