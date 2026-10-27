StudyFlow Android APK project
=============================

මෙය ඔබේ hosted StudyFlow වෙබ් ඇප් එක Android WebView ඇප් එකක් ලෙස විවෘත කරන project එකකි.
මෙය APK ගොනුව නොව APK එක build කිරීමට අවශ්‍ය source project එකයි.

ලේසිම ක්‍රමය: GitHub Actions හරහා APK build කිරීම
-------------------------------------------------
1. https://github.com වෙත ගොස් ඔබේ account එකට sign in වෙන්න.
2. New repository එකක් සාදන්න. උදාහරණයක්: StudyFlow-APK
3. මේ ZIP එකේ ඇතුළත තියෙන සියලුම ගොනු repository එකට upload කරන්න. (ගොනු ඇතුළත ගොනු/hidden .github folder එකත් ඇතුළත් විය යුතුයි.)
4. repository එකේ Actions tab එකට යන්න.
5. "Build StudyFlow APK" workflow එක පෙනේ නම් එය තෝරා Run workflow ඔබන්න.
   පළමු push එකෙන් build එක ස්වයංක්‍රීයව ද පටන් ගත හැක.
6. Build එක සාර්ථක වූ පසු Actions තුළ අදාළ run එක විවෘත කරන්න.
7. Artifacts කොටසෙන් "StudyFlow-APK" download කරන්න.
8. ZIP file එක extract කර app-debug.apk ගොනුව Android phone එකට යවන්න.
9. APK එක විවෘත කර install කරන්න. Android විසින් browser/unknown-source අවසරයක් අසන්නේ නම්, ඔබ විශ්වාස කරන මේ APK එකට පමණක් අවසර දෙන්න.

වැදගත්:
- APK එක load වීමට internet සම්බන්ධතාවයක් අවශ්‍යයි; මෙය offline app එකක් නොවේ.
- StudyFlow හි local storage දත්ත Android WebView එකේ වෙනම save වේ. Chrome browser එකේ දත්ත APK එකට ස්වයංක්‍රීයව මාරු නොවේ.
- App data clear කළොත් හෝ app එක uninstall කළොත් එහි local study data නැති විය හැක. වැදගත් දත්ත සඳහා app එකේ export/backup පහසුකම තිබේ නම් එය භාවිතා කරන්න.
- මෙය personal testing සඳහා debug APK එකකි; Google Play Store publish කිරීම සඳහා release signing සහ අදාළ Play Store requirements වෙනම අවශ්‍ය වේ.
- පළමු build එකෙන් පසු APK එක install කර Timer, task save, theme, navigation, PDF download වගේ දේවල් phone එකේ test කරන්න.
