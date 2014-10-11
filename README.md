liteTranslate
=============

Not just another approach of Google Translate API

##Intro  
One-Click/Touch based translate is a very common approach to translating app on the web and touch devices. The mechanism behinds the approach was:  
  1. query (part of) the page to the server  
  2. use server appliction to parse the page in order to add an identical tag to each word  
  3. send parsed page back to the client
  4. Page is powerred with JS to add event listener on all identical tag to show a translate qtip with the help of Google Translate API

Someone would have wonderred, why don't just query the page on the front end, and add event listener to all word on the page? The reason was: double is needed, for instance, window.getSelection() to get the range the word. So either you changed the approach to Doube-Click/Touch based translate, like how Google did with its native Goolge Dictionary app, or you add an identical tag to the word, like in former approach, which is used by a very popular app Tap-Translate. 

##The New Approach
Kudos to the previous approached, it works great, but an obstacle was avoided, and I can't stand that.

Here is my approach: everything at once, every on step 4. 
