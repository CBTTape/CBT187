# CBT187
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 187 WAS FROM THE FIRST NATIONAL BANK OF CHICAGO, AND HAS  *   FILE 187
//*           BEEN SIZABLY UPDATED BY SAM GOLOB.  THE "CVTCLIST"    *   FILE 187
//*           OR "CONVERT CLIST" PROGRAM CONVERTS ENTIRE            *   FILE 187
//*           CLIST LIBRARIES FROM EITHER THE FB-80 FORMAT TO       *   FILE 187
//*           THE VB-255 FORMAT OR VICE-VERSA.  GUESSWORK IS        *   FILE 187
//*           ELIMINATED, AND THE CONVERSION IS QUICK, AT ASSEMBLER *   FILE 187
//*           SPEED.  ESPECIALLY USEFUL IS THE VB-FB CONVERSION.    *   FILE 187
//*                                                                 *   FILE 187
//*   Note:  For logic to convert REXX execs from VB-255 to         *   FILE 187
//*          FB-80 format, please see the REXX8080 member of        *   FILE 187
//*          File 155.                                              *   FILE 187
//*                                                                 *   FILE 187
//*           THIS CODE HAS BEEN MODIFIED BY SAM GOLOB TO LEVEL     *   FILE 187
//*           V2R3M1 WITH KNOWN BUGS FIXED, AND WITH THE "LONG      *   FILE 187
//*           LINES" OF THE "255 FORMAT" PROPERLY FOLDED, SO THAT   *   FILE 187
//*           THE CONVERTED CLISTS EXECUTE IDENTICALLY TO THE WAY   *   FILE 187
//*           THE ORIGINAL CLISTS EXECUTED.  BUT REXX PROGRAMS      *   FILE 187
//*           WILL STILL HAVE TO BE EXAMINED BY HAND AFTER THE      *   FILE 187
//*           CONVERSION.  THIS PROGRAM WILL MAKE THAT PROCESS      *   FILE 187
//*           EASIER, BECAUSE IT FLAGS ALL MEMBERS WHICH HAD        *   FILE 187
//*           LONG LINES SPLIT, AND TELLS YOU HOW MANY SPLITS       *   FILE 187
//*           WERE DONE IN EACH MEMBER.  YOU'LL JUST HAVE TO        *   FILE 187
//*           LOOK AT EACH EXEC AND SEE WHICH LINES HAVE BEEN       *   FILE 187
//*           SPLIT "CLIST-STYLE".                                  *   FILE 187
//*                                                                 *   FILE 187
//*           THIS PROGRAM MAKES IT POSSIBLE TO EASILY CONVERT      *   FILE 187
//*           THE CLIST FORMATS OF ANY SHOP.  NOW, YOU ARE NOT      *   FILE 187
//*           "FROZEN" IN ANY ONE CLIST FORMAT.                     *   FILE 187
//*                                                                 *   FILE 187
//*           DEFAULT EXECUTION OF THIS PROGRAM IS TO REPLACE       *   FILE 187
//*           EXISTING MEMBERS IN THE OUTPUT LIBRARY.  IF YOU       *   FILE 187
//*           DON'T WANT TO REPLACE EXISTING MEMBERS, EXECUTE       *   FILE 187
//*           THE PROGRAM WITH PARM=ADD.                            *   FILE 187
//*                                                                 *   FILE 187
//*           THIS LEVEL OF THE CONVERT CLIST PROGRAM "CVTCLIST"    *   FILE 187
//*           HAS BEEN FIXED TO BECOME "THE" TOOL FOR ACCOMPLISHING *   FILE 187
//*           EASY CLIST PROGRAM CONVERSIONS BETWEEN THE TWO        *   FILE 187
//*           INCOMPATIBLE DCB FORMATS.                             *   FILE 187
//*                                                                 *   FILE 187
//*           SYSUT1 IS THE INPUT DDNAME AND SYSUT2 IS THE OUTPUT   *   FILE 187
//*           DDNAME FOR THIS PROGRAM.  THEY MUST BE OF DIFFERENT   *   FILE 187
//*           CLIST DCB FORMATS FROM EACH OTHER.  ONE DDNAME MUST   *   FILE 187
//*           BE FB-80 AND THE OTHER MUST BE VB-255.  ALL MEMBERS   *   FILE 187
//*           OF THE LIBRARY POINTED TO BY SYSUT1 WILL BE COPIED    *   FILE 187
//*           TO CONVERTED (AND RENUMBERED) MEMBERS IN THE SYSUT2   *   FILE 187
//*           LIBRARY.  THE PROGRAM FIGURES OUT FROM THE DCB        *   FILE 187
//*           INFORMATION OF EACH FILE, WHICH WAY TO DO THE         *   FILE 187
//*           CONVERSION.                                           *   FILE 187
//*                                                                 *   FILE 187
//*           THIS LEVEL OF CVTCLIST ALLOWS MEMBER REPLACEMENT TO   *   FILE 187
//*           TAKE PLACE IN THE SYSUT2 LIBRARY.  THAT PREVIOUSLY    *   FILE 187
//*           WAS NOT ALLOWED.  FORMERLY, THE SYSUT2 LIBRARY HAD    *   FILE 187
//*           TO BE EMPTY.  THE SYSPRINT DDNAME GIVES A REPORT      *   FILE 187
//*           SHOWING HOW MANY MEMBERS WERE ADDED TO THE SYSUT2     *   FILE 187
//*           DATASET, AND HOW MANY MEMBERS WERE REPLACED.          *   FILE 187
//*                                                                 *   FILE 187
//*           FOR VB-255 TO FB-80 CONVERSIONS, WHERE LONG LINES     *   FILE 187
//*           ARE SPLIT, ISPF STATISTICS ARE NOW ADJUSTED TO ADD    *   FILE 187
//*           THE NUMBER OF LINE SPLITS TO THE SIZE, PROVIDED THAT  *   FILE 187
//*           ISPF STATISTICS EXISTED FOR THE MEMBER IN THE FIRST   *   FILE 187
//*           PLACE.  IF THEY DIDN'T EXIST FOR A MEMBER, NOTHING    *   FILE 187
//*           IS DONE TO THE DIRECTORY ENTRY.                       *   FILE 187
//*                                                                 *   FILE 187
//*           NOW, WITH THIS CVTCLIST VERSION, IT IS POSSIBLE TO    *   FILE 187
//*           MERGE SEVERAL CLIST LIBRARIES WHILE CONVERTING        *   FILE 187
//*           THEM, BECAUSE MEMBER REPLACEMENT IS NOW ALLOWED.      *   FILE 187
//*                                                                 *   FILE 187
//*           NOW ALSO, WHEN CONVERTING VB-FB, ALL NUMERICS         *   FILE 187
//*           IN COLUMNS 81-88 ARE FLAGGED AND COUNTED, BECAUSE     *   FILE 187
//*           THEY MAY BE SPURIOUS SEQUENCE NUMBERS LEFT OVER       *   FILE 187
//*           AFTER A PREVIOUS FAULTY CONVERSION FROM FB TO VB.     *   FILE 187
//*           IF THERE WAS DATA IN COLUMNS 1-8, 73-80 ARE CHECKED   *   FILE 187
//*           TO SEE IF THEY ARE NUMERIC, INSTEAD OF 81-88.         *   FILE 187
//*                                                                 *   FILE 187
//*           AT THE PRESENT LEVEL, THE PROGRAM DOES NOT "STRIP"    *   FILE 187
//*           THESE NUMBERS OUT AND CONVERT THEM TO BLANKS.  IT     *   FILE 187
//*           MAY DO SO IN THE NEAR FUTURE UNDER CONTROL OF A       *   FILE 187
//*           PARM.  IF YOU REALLY WANT THE PROGRAM TO STRIP THESE  *   FILE 187
//*           NUMERICS OUT, YOU JUST HAVE TO UNCOMMENT ONE          *   FILE 187
//*           INSTRUCTION.                                          *   FILE 187
//*                                                                 *   FILE 187
```
