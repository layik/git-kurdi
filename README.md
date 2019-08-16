# Git-kurdi

------

دەربارە: ئەم فێرکاریەی گیت وەرگێڕانێکی ئەم دەقە [سەرچاوەکراوەیە](https://github.com/pluralsight/git-internals-pdf) بوو له‌ ٢٠١١ و زووتریش ده‌ستم پێكرد. هیوادارم كه‌سێك\كه‌سانێك. لە ئێستادا کاک [ڕەوەند](https://github.com/rawandsaeed) خۆی دەستپێشخەری کرد کە ئەرک بکێشێ، بیگەیەنینە ئەنجام.

جا ڕیپۆ ئەسڵیەکە ماشەڵا ئەستێرەی دنیای گرتوە، بەڵکە کوردیەکەش وابێت. دڵنیام ئەوانیش خۆشحاڵەبن وەرگێڕانەکە ببین.

له‌م ڕیپۆیه‌ هه‌وڵ ده‌ده‌ین كه‌ به‌ش به‌ش ته‌واو بێت چونكه‌ وه‌ڕگێرانه‌كه‌ ته‌واو نه‌بوه‌ له‌ ئێستادا. 

له‌ به‌شی ناوه‌ڕۆك ده‌توانین بیبینیت كه‌ چ به‌شێك ته‌واو بووه‌ بۆ ئه‌وه‌ی بتوانیت بیخوێنیته‌وه‌.



## ناوه‌ڕۆك

*تێبینی: ئه‌وبه‌شانه‌ی كه‌ لینك نین ئه‌وانه‌ن كه‌ ته‌واو نه‌بوون هێشتا. به‌شاكانی تر ده‌توانین كلیكیان بكه‌یت و به‌خوێنیته‌وه‌.* 



٣ **[مێژوویه‌كی كورتی گیت](https://github.com/layik/git-kurdi/blob/master/به%E2%80%8Cشه%E2%80%8Cكان/مێژوویه%E2%80%8Cكی%20كورتی%20گیت.md)**

٤ **[ده‌رباره‌ی ئه‌م كتێبه‌](https://github.com/layik/git-kurdi/blob/master/به%E2%80%8Cشه%E2%80%8Cكان/ده%E2%80%8Cرباره%E2%80%8Cی%20ئه%E2%80%8Cم%20كتێبه%E2%80%8C.md)**

٥ **[دامه‌زراندی گیت](https://github.com/layik/git-kurdi/blob/master/به%E2%80%8Cشه%E2%80%8Cكان/دامه%E2%80%8Cزراندنی%20گیت.md)**

٥ دامه‌زراندن له‌ لینوكس

٦ دامه‌زراندن له‌ ماك

٧ ویندۆس

٨ مێژوویه‌كی كورتی گیت



١٠ **[تێگه‌یشتن له‌ گیت](https://github.com/layik/git-kurdi/blob/master/به%E2%80%8Cشه%E2%80%8Cكان/تێگه%E2%80%8Cیشتن%20له%E2%80%8C%20گیت.md)**

١٠ گیت چیه‌؟

١١ فۆكس و دیزاین

١٣ جۆری ته‌نی گیت

٢٢ مۆدێلی داتای گیت

٢٨ برانچین و مێرجین

٤١ دار

٤٤ دایرێكته‌ری گیت

٤٨ ئیشكردن له‌ دایرێكته‌ری

٤٩ ئیندێكس



٥٤ **[به‌كارهێنانی گیت](https://github.com/layik/git-kurdi/blob/master/به%E2%80%8Cشه%E2%80%8Cكان/بەکارهێنانی%20گیت.md)**

٥٤ پێكهێنانی پرۆفایل

٥٥ بردن بۆ ریپۆی گیت

٥٧ نموونه‌ی ئیشكردنی نۆرماڵ

٦٣ لۆگ- مێژووی كۆمیت

٦٥ براوسین له‌ گیت

٧١ گه‌ڕان له‌ گیت

٧٢ گیت دیف (جیاوازی)

٧٥ برانچین

٧٧ مێرجینێكی ساده‌

٨٠ ڕیبه‌سه‌ین

٨٦ ستراشین 

٨٩ تاگین

٩١ هاویشتنه‌ ده‌ره‌وه‌ی گیت

٩٢ ئاگاداربوون له‌ گیت

٩٤ نموونه‌ی ئیشكردنی دیستریبیوتید 

١٠٥ شێری ریپۆكان

١٠٧ ریپۆ هۆستكراوه‌كان



١١١ **پوخته‌ی كۆماند**

١١١ گیتی سه‌ره‌تای

١١٥ پشكنینی ریپۆكان

١١٧ كه‌ره‌سته‌ی زیاتر



١١٩ **سه‌رچاوه‌ و ژێده‌ره‌كان**

١١٩ دۆكیۆمێنتی وێب

١٢٠ سكرین شۆت



١٢١ **پێداچوونه‌وه‌**



## فۆرماتی فایله‌كان

- دكتۆر له‌یك سه‌ره‌تا ده‌قه‌كه‌ی به‌ HTML  نووسیوه‌ كه‌ كاتی زۆر ده‌وێت و كێشه‌ی زۆره‌ وه‌ك له‌ ماركداون هه‌ربۆیه‌ كاك ڕه‌وه‌ند ده‌قه‌كه‌ی له‌ HTML گۆڕیوه‌ بۆ ماركداون كه‌ پشتگه‌ری نووسینی ڕاست بۆ چه‌پ ده‌كات. 
- له‌ ئێستادا‌ فۆرماتی ده‌قه‌كه‌ به‌ ماركداونه‌.
- له‌ داهاتوودا كه‌ ته‌واو بوو ده‌یكه‌ین به‌ PDF
- به‌رنامه‌ی ماركداون به‌ به‌رنامه‌ی [Typora‌](https://typora.io) كه‌ پشتیوانی RTL (نووسین له‌ ڕاسته‌وه‌ بۆ چه‌پ) ده‌كات و زۆر ئاسانه‌ به‌كارهێنانی وه‌ هه‌روه‌ها بۆ هه‌ر سێ سیسته‌مه‌كه‌ دابه‌زاندنی هه‌یه‌: بۆ زانیاری زیاتر كلیك بكه‌ له‌سه‌ر لینكی سه‌روو. 
- كاتێك كه‌ به‌رنامه‌كه‌ت دابه‌زاند ده‌توانین په‌ڕه‌ی [Middle East](http://theme.typora.io) به‌كاربهێنیت بۆ نووسینی كوردی له‌ ماك و ویندۆس و لینۆكس. 
- ده‌توانیت به‌ به‌رنامه‌ی ماركداونی تر ئیش بكه‌یت كه‌ بتوانێت پشتگیری RTL بكات. 



## چۆن ده‌توانیت یارمه‌تی بده‌یت

ده‌توانیت فۆرك بكه‌یت و برانچێك دروست بكه‌یت بۆ هه‌ر كۆمه‌تێك ده‌توانیت پووڵ بكه‌یت بۆ ئه‌وه‌ی دوای مێرجی بكه‌ین. ده‌توانیت ڕاسته‌وخو كۆمیت بكه‌ت له‌ ڕیپۆكه‌ به‌ڵام ئه‌م ڕێگایه‌ زۆر باش نیه‌ بۆ ئاسانی خاوه‌نی رێپۆكه‌ ئه‌و كاره‌ ده‌كات باشتره‌. 



به‌م ڕێگایه‌نه‌ ده‌توانیت یارمه‌تی بده‌یت بۆ ئه‌م ته‌واوكردنی ئه‌م پڕۆجێكته‌:

- وه‌ڕگێرانی ئه‌وبه‌شانه‌ی كه‌ وه‌رنه‌گێڕاون.
- ڕاستكردنه‌وه‌ی ووشه‌كان. 
- ئه‌وه‌نده‌ی ده‌توانین له‌ شوێنی خۆیدا ووشه‌ی كوردی به‌كاربهێنین.
- وه‌ك بزانین ئه‌مه‌ تاكه‌ شوێنه‌ كه‌ باس له‌ گیت بكرێت به‌ زمانی كوردی بۆیه‌ ته‌واو كردنی ئه‌م پڕۆژه‌ گرنگریه‌كی زۆری هه‌یه‌ بۆ زۆر كه‌س و كه‌سانی تازه‌. 
- [كتێبه‌كه‌](https://github.com/layik/git-kurdi/blob/master/peepcode-git.pdf)‌ به‌ زمانی ئینگلیزی. 