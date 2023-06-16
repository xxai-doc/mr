<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

वेबसाइट कोडचा एक भाग मुक्त स्रोत आहे, भाषांतर ऑप्टिमाइझ करण्यात मदत करण्यासाठी आपले स्वागत आहे.

## फ्रंट-एंड कोड

* [फ्रंट-एंड कोड](https://github.com/xxai-art/web)
* [संपूर्ण साइटसाठी भाषा पॅक](https://github.com/xxai-art/web/tree/main/i18n)
* [लॉगिन मॉड्यूलसाठी भाषा पॅक](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [वेबसाइट बहुभाषिक दस्तऐवजीकरण](https://github.com/xxai-doc)

फ्रंट-एंड प्रोग्रामिंग भाषा [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) आहे, जी कॉफीस्क्रिप्ट सिंटॅक्सवर आधारित काही वैशिष्ट्ये जोडते, पहा [./coffee_plus.md](./coffee_plus.md) .

## वेबसाइट्स आणि दस्तऐवजांचे आंतरराष्ट्रीयीकरण

खालील 3 प्रकल्पांवर तयार करा

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  प्रत्यय आहे `.mdt` , तुम्ही बाह्य फाइल्सचा संदर्भ देण्यासाठी `<+ ./coffee_plus/import.js>` सारखा वाक्यरचना वापरू शकता आणि प्रत्यय `.md` सह मार्कडाउन तयार करू शकता.

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  मार्कडाउन भाषांतर कोड आणि लिंक्सचे भाषांतर करणार नाही आणि अनुवादित वाक्ये कॅशे करेल. जर अनुवाद सुधारित केला असेल परंतु मूळ मजकूर सुधारला नसेल, तर तो पुन्हा कार्यान्वित केल्याने भाषांतरातील बदल ओव्हरराईट होणार नाहीत.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` व्युत्पन्न केलेल्या वेबसाइट्सचे भाषांतर करण्यासाठी भाषा फाइल्स.
