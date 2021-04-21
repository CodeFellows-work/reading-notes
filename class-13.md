# Local Storage # 
Having a database within your web page will make your web page more alpha than a web page that might not have a local database or storage. Simply put, you can do a lot more with storage. 
Having storage within your web page can improve the performance of your web page. One of the reasons for this is because every HTTP request that is made on your page, cookies are included. The maximum cookies you can have is limited to only 4KB of data. If it gets to this point you will notice that your web applicatioon or page will start to run very slowly. 
### History ### 
So to solve the space issue within browsers in the early daays, Microsoft developed something called userData with Internet Explorer. This allowed web pages to store up to 64KB of data per domain. 

Some time later, Adobe introduced a feature that came along with Flash 6. This basically allowed Flash objects to store up to 100KB of data per domain. 

Then you have someone named Brad Neuberg. Brad, was able to develop something called AMASS, which was a Flash to JavScript connection. Sometime later, Brad was able to update the AMASS and merge it with something called the DojoToolkit which allowed Flash to store the 100KB per domain for free. 

In 2007, Google came up with something. That something was called Gears. This was an open sourced plugin and provided additional capabilities to browsers with this plug in. If you know the Google Maps APIs you will know this. Gears basically stored data with an SQL based database. 


### HTML5 Storage ###
After sometime later, we have HTML5 storage. HTML5 storage is basically supported by all browsers used today and does not need a third party plug in. So to use HTML5 storage within your HTML you will need to use the `localStorage` object within the global `window` object to check for HTML5 Storage. This is an example: 

            function supports_html5_storage() {
      try {
        return 'localStorage' in window && window['localStorage'] !== null;
      } catch (e) {
        return false;
      }
    }
    
    Source: http://diveinto.html5doctor.com/storage.html
    
Or you can use **Modernizer** to do this: 

            if (Modernizr.localstorage) {
        // window.localStorage is available!
      } else {
        // no native support for HTML5 storage :(
        // maybe try dojox.storage or a third-party solution
      }
      
    Source: Source: http://diveinto.html5doctor.com/storage.html
    
So to use the HTML5 storage you need to understnad that it will store data as a string. You can still put in various data types such as booleans, Numbers, strings, or floats, but you will need to use functions to translate them out of a string. 

So This is how HTML5 storage can look like if you want to maybe save a game: 

          function saveGameState() {
        if (!supportsLocalStorage()) { return false; }
        localStorage["halma.game.in.progress"] = gGameInProgress;
        for (var i = 0; i < kNumPieces; i++) {
      localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
      localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
        }
        localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
        localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
        localStorage["halma.movecount"] = gMoveCount;
        return true;
    }
    
    Source: http://diveinto.html5doctor.com/storage.html
    
A big thing to note is that this is all storage using key/value pairs. 
