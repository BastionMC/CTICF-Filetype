THIS README IS TEMPORARY AND RIPPED STRAIGHT FROM
BASTIONCMD's UI.CTICF FILE!! REPLACE LATER!!!
                
                
                
                Yo, this is our own format!

  Short explanation:
  
    $$ : Text gets inserted by the program here
    
    §§[r|g|y|b|m|c|w,0][d|n|b][f,b] : The text color will
                                        be changed by this!
    
        [red,green,yellow,blue,magenta,cyan,white,black]
        [dim,normal,bright]
        [foreground,background]
        
        (Only pick one of the letters in
        the list! For sample "§§rnf"!)
        
    §$ : Reset text color
    
    $§ : Split text segments

 ──────────────────────────────────────────────────────────────

     Texts are referred to by index! If you add anything,
     please do that at the bottom! It saves a lot of time,
     trust me.
     
     There is a chance your syntax will get misread by the
     interpreter. To avoid this, leave a space inbetween
     each control-character-combination ($$,§§,§$,$§).
     
     The interpreter allows for unecessary whitespaces to
     be inbetween the different strings, as it will get
     trimmed. If you want the whitespace formatting, you
     will have to do that through code, sorry.
     
     Please pay attention to the line length when adding
     texts! To follow the style, use a maximum of 64 chars
     per line!
 
 ──────────────────────────────────────────────────────────────
 
        https://www.github.com/BastionMC/CTICF-Filetype
 
 ──────────────────────────────────────────────────────────────

  You can comment the beginning of files! Use a Hashtag to
  indicate that the actual data is starting. Do not use it
  multiple times in a file, or else only the parts after the
  last hashtag will get read!

#
