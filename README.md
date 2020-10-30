<h1 id="top">Medtouch Applications</h2>

##### These are the applications built and deployed during my work at [Medtouch](https://www.medtouch.com.br).  During these over 8 years, I've built over 10 apps for the [iOS Platform](#appios) and 5 for the [Android Platform](#appandroid) and the respective app updates for both platforms.

##### It is worth mentioning the "timing", i.e., some features that with the current tools and frameworks are trivial to do, was done/built "manually" and I'll present this as it was at that time (innovative, difficult to accomplish, etc).

### iOS: 

&nbsp;&nbsp; [![AppStore](icons/apple-badge-black.png "AppStore")](https://tinyurl.com/y4qs4c9l)<br>

&nbsp;&nbsp; [![Code Blue](icons/Icon_CodeBlue_60.png "Code Blue - iOS")](#codeblue)  [![Condutas](icons/Icon_Conds60.png "Condutas em Emergência")](#condutas)  [![Dengue](icons/Icon_Dengue_60.png "Dengue - iOS")](#dengue)  [![DocCalc](icons/Icon_DocCalc_60.png "DocCalc - iOS")](#doccalc)  [![DrAureo](icons/Icon_DrAureo_60.png "Dr Aureo - iOS")](#draureo)  [![Drogas](icons/Icon_Drogas_60.png "Drogas em Emergência & CTI - iOS")](#drogas)  [![Eponimos](icons/Icon_Epons-60.png "Epônimos")](#epons)  [![GravLact](icons/Icon_GravLact_60.png "Gravidez e Lactação")](#gravlact)  [![GuiaATMs](icons/Icon_GuiaATMs-60.png "Guia de Antimicrobianos")](#guiaatms)  [![PrescMed](icons/Icon_Presc_60.png "Prescrições Médicas")](#prescs)

### Android: 

[![Google Play](icons/google-play-badge.png "Google Play")](https://shorturl.at/fyFMQ)<br>

&nbsp;&nbsp; [![Code Blue](icons/Icon_CodeBlue_60.png "Code Blue - Android")](#codeblueA)  [![Dengue](icons/Icon_Dengue_60.png "Dengue - Android")](#dengueA)  [![DocCalc](icons/Icon_DocCalc_60.png "DocCalc - Android")](#doccalcA)  [![DrAureo](icons/Icon_DrAureo_60.png "Dr Aureo - Android")](#draureoA)  [![Drogas](icons/Icon_Drogas_60.png "Drogas em Emergência & CTI - Android")](#drogasA)


<h2 id="appios">iOS Applications:</h3>
Most of the applications for the iOS platform were built in Objective-C, using all different types of tools and frameworks available at the time<br>I'll try to show the main features of each one and what can be done to improve them.

[Back to Top](#top)
----

<img id="codeblue" align="left" src="icons/Icon_CodeBlue_60.png"><b>Code Blue</b><br>The most complete application of Intensive Care Medicine in Brazil, developed by specialist doctors qualified by AMIB!
<br>

### Features: 
1. Built using Objective-C language;
2. Use of custom table view index, using the first three letters of the category and javascript commands inside the objective-C code (use of search bar to find and highlight keywords in the text);<br>
![Temas](CodeBlue/gifs/Temas1.gif "Temas")
3. Use of the FPPopover and MFSideMenu libraries on the first tab, the first to create a Popover with the topics of text and the second to create a Side Menu ("drawer");<br>
![Drogas](CodeBlue/gifs/Drogas.gif "Drogas")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![SideMenu](CodeBlue/gifs/SideMenu.gif "SideMenu") 
4. 88 Calculators, 201 Drugs and 119 Trials(Article summaries) built using HTML/CSS/Javascript and wrapped in a webview;<br>
![Calcs](CodeBlue/gifs/Calcs1.gif "Calcs")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Trials](CodeBlue/gifs/Trials.gif "Trials")
5. A Note Taking tab, where you can save your simple notes for future consultation;<br>
![Calcs2Nota](CodeBlue/gifs/Calcs2Nota.gif "Calcs2Nota")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Nota](CodeBlue/gifs/Notas.gif "Nota")

### Improvements:
1. Most of the app's content is in html format, accessed through property lists with title and file name. A suggestion to improve the performance and security of the app is to put these files in a real database, with all its access control and security features and generate each html file at time of use;
2. In addition, greater attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;

[Back to Top](#top)
----

<img id="condutas" align="left" src="icons/Icon_Conds60.png"><b>Condutas em Emergências</b><br>Your emergency shifts will be calmer now. Fast and reliable information on more than 30 serious diseases!
<br>

### Features:
1. Built using Objective-C language;
2. For this application, all the content was already divided into hundreds of PDF files, so to increase productivity, it was decided to use these files wrapped in a WebView;
3. Traditional app, consisting of a TabViewController in which each tab is a TableView with its respective Detail View Controller;<br>
![Condutas](Condutas/gifs/Condutas.gif "Condutas")
4. In the case of the Calculators Tab, a UISegmentedControl was used to switch the display of calculators between "All calculations" and "By Category". In this case, the customized index was chosen, with the initial letters of each category;<br>
![Calcs](Condutas/gifs/Calcs.gif "Calcs")
5. A great feature implemented in the app, to serve a large number of users who have requested this is the possibility to take notes;<br>
![CondsCalcsNotas](Condutas/gifs/CondsCalcsNotas.gif "CondsCalcsNotas")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Notas](Condutas/gifs/Notas.gif "Notas")
6. Another interesting feature of this app is the possibility to save conducts as favorites;<br>
![CondutasFav](Condutas/gifs/CondutasFav.gif "CondutasFav")&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Favs](Condutas/gifs/Favs.gif "Favs")


### Improvements:
1. As all the content was in pdfs, and used as so, a suggestion to improve the performance and security of the app is to put their content in a database, with all its access control and security features and generate each html file at time of use;
2. Think in transitioning the code to Swift;
3. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
4. Here, again, more attention should be paid to UI/UX;
5. Improvements on Autolayout implementations must be done;

[Back to Top](#top)
----

<img id="dengue" align="left" src="icons/Icon_Dengue_60.png"><b>Dengue</b><br>Diagnostic and therapeutic management guide for adults and children prepared by the Ministry of Health.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features:
1. Built using Objective-C language and updated to Swift;
2. The app consists of a TabViewController with 5 tabs, where the first four are webviews with the Html/CSS/Bootstrap/JS/jQuery app on it and the same feature of the app **Code Blue** (to create a list with the titles in the text, for quick access) was done, but in this case it was built with Html/CSS/Bootstrap/JS/jQuery resources;<br>
![Tab5_Share](Dengue/gifs/Tab5_share.gif "Tab5_Share")
3. The fifth tab ("share") of the app consists in a TableView Object where each row provide a different link to the company on internet, like social networks (Twitter or Facebook), the Developer's website, to an online registration form or to send an email to the company and in the upper right there is a button that opens a View with the other apps of the developer;<br>
![Tabs_Titles](Dengue/gifs/Tabs_Titles.gif "Tabs_Titles")

### Improvements:
1. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
2. Here, again, some stuff to do in UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
5. One radical change suggested by some executives of the developer is to switch to an cross-platform approach, using the same base of the Android App, that way the resources would be better used;

[Back to Top](#top)
----

<img id="doccalc" align="left" src="icons/Icon_DocCalc_60.png"><b>DocCalc</b><br>More than 300 medical calculations, with algorithms, scores, unit converters, classifications, formulas, diagnostic and prognostic criteria, to assist in your medical practice.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. All the content is in html files, a suggestion to improve the performance and security of the app is to put their content in a database, with all its access control and security features and generate each html file at time of use;
2. Think in transitioning the code to Swift;
3. Here, again, more attention should be paid to UI/UX;
4. Improvements on Autolayout implementations must be done;
5. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
6. One radical change suggested by some executives of the developer is to switch to an cross-platform approach, using the same base of the Android App, that way the resources would be better used;

[Back to Top](#top)
----

<img id="draureo" align="left" src="icons/Icon_DrAureo_60.png"><b>Dr Aureo</b><br>Application for Dr. Aureo's patients. Various information about your doctor. Tips on health and medical examinations, calculations (BMI, ideal weight, etc.) and recommendations from professionals in other specialties.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built in Html/CSS/JS, using Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Think in transitioning the code to Swift;
2. Here, again, more attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
5. One radical change suggested by some executives of the developer is to switch to an cross-platform approach, using the same base of the Android App, that way the resources would be better used;

[Back to Top](#top)
----

<img id="drogas" align="left" src="icons/Icon_Drogas_60.png"><b>Drogas em Emergência & CTI</b><br>A quick reference guide with the main drugs used in emergency and intensive care, made by physicians who work "on the front line"!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. 4 Idioms: PT, EN, ES, CH;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
4. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. All the content is in .plist files, a suggestion to improve the performance and security of the app is to put their content in a database, with all its access control and security features;
2. Think in transitioning the code to Swift;
3. Here, again, more attention should be paid to UI/UX;
4. Improvements on Autolayout implementations must be done;
5. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;

[Back to Top](#top)
----

<img id="epons" align="left" src="icons/Icon_Epons-60.png"><b>Epônimos</b><br>THE WORLD'S MOST COMPLETE APP IN THE GENDER! More than 4000 terms in Medicine, Dentistry, Nutrition, Physiotherapy and Nursing!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Think in transitioning the code to Swift;
2. Here, again, more attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;

[Back to Top](#top)
----

<img id="gravlact" align="left" src="icons/Icon_GravLact_60.png"><b>Gravidez e Lactação</b><br>A reliable guide containing Conducts, Calculators and Drug Guide for the management of pregnant and lactating women, in a FRIENDLY INTERFACE!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Think in transitioning the code to Swift;
2. Here, again, more attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;

[Back to Top](#top)
----

<img id="guiaatms" align="left" src="icons/Icon_GuiaATMs-60.png"><b>Guia de Antimicrobianos</b><br>Therapeutic indications for more than 500 infections, in adults and children; Surgical prophylaxis; Pharmacological Guide; 180 Most common bacteria, calculators, etc.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Think in transitioning the code to Swift;
2. Here, again, more attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;

[Back to Top](#top)
----

<img id="prescs" align="left" src="icons/Icon_Presc_60.png"><b>Prescrições Médicas</b><br>A true EVIDENCE-BASED medical prescriptions guide, written by SPECIALIST DOCTORS!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Objective-C language;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Think in transitioning the code to Swift;
2. Here, again, more attention should be paid to UI/UX;
3. Improvements on Autolayout implementations must be done;
4. Change the architecture MVC to MVVM and refactor the code to make it easy to build Tests;
5. One radical change suggested by the executives guys is to switch to an cross-platform approach, using the same base of the Android App, that way the resources would be better used;

[Back to Top](#top)
----

<h2 id="appandroid">Android Applications:</h2>
These applications were done in HTML/CSS/JS/jQuery/Bootstrap and using cross-platform tools like Intel XDK, PhoneGap and Apache Cordova to wrap into native builds!<br>I'll try to show the main features of each one and what can be done to improve them.

[Back to Top](#top)
----

<img id="codeblueA" align="left" src="icons/Icon_CodeBlue_60.png"><b>Code Blue</b><br>The most complete application of Intensive Care Medicine in Brazil, developed by doctors qualified by AMIB!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Html, CSS, Bootstrap, JS, jQuery and using Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
2. Put each and every one button to work properly;
3. Authentication for the users in Firebase;

[Back to Top](#top)
----

<img id="dengueA" align="left" src="icons/Icon_Dengue_60.png"><b>Dengue</b><br>Diagnostic and therapeutic management guide for adults and children prepared by the Ministry of Health.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built in Html/CSS/JS, using, firstly, Intel XDK, then Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Make the necessary adaptations to integrate the iOS and Android versions in a single app;
2. Here, again, more attention should be paid to UI/UX;

[Back to Top](#top)
----

<img id="doccalcA" align="left" src="icons/Icon_DocCalc_60.png"><b>DocCalc</b><br>More than 300 medical calculations, with algorithms, scores, unit converters, classifications, formulas, diagnostic and prognostic criteria, to assist in your medical practice.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built in Html/CSS/JS, using, firstly, Intel XDK, then Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

[Back to Top](#top)
----

<img id="draureoA" align="left" src="icons/Icon_DrAureo_60.png"><b>Dr Aureo</b><br>Application for Dr. Aureo's patients. Various information about your doctor. Tips on health and medical examinations, calculations (BMI, ideal weight, etc.) and recommendations from professionals in other specialties.
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Html, CSS, Bootstrap, JS, jQuery and using Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Make the necessary adaptations to integrate the iOS and Android versions in a single app;
2. Here, again, more attention should be paid to UI/UX;

[Back to Top](#top)
----

<img id="drogasA" align="left" src="icons/Icon_Drogas_60.png"><b>Drogas em Emergência & CTI(4 Idioms: PT, EN, ES, CH)</b><br>A quick reference guide with the main drugs used in emergency and intensive care, made by physicians who work "on the front line"!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built using Html, CSS, Bootstrap, JS, jQuery and using Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Make the necessary adaptations to integrate the iOS and Android versions in a single app;
2. Here, again, more attention should be paid to UI/UX;

[Back to Top](#top)
----

### Obs:
The app can be seen [here](https://tinder-clone-c1a91.web.app)

[Back to Top](#top)
----

<img id="prescsA" align="left" src="icons/Icon_Presc_60.png"><b>Prescrições Médicas</b><br>A true EVIDENCE-BASED medical prescriptions guide, written by SPECIALIST DOCTORS!
<br>
<br>
[![Under Construction](AnimGifs/UnderConstructionBelow.gif "Under Construction")](#underconstruction) 
<br>
### Features: 
1. Built in Html/CSS/JS, using, firstly, Intel XDK, then Apache Cordova to wrap in native code;
2. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;
3. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat;

### Improvements:
1. Make the necessary adaptations to integrate the iOS and Android versions in a single app;
2. Here, again, more attention should be paid to UI/UX;

[Back to Top](#top)
----

iOS Applications           |  Android Applications
:-------------------------:|:-------------------------:
[![AppStore](icons/apple-badge-black.png "AppStore")](https://tinyurl.com/y4qs4c9l) | [![Google Play](icons/google-play-badge.png "Google Play")](https://shorturl.at/fyFMQ)
