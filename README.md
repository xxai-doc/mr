<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

डिरेक्टरी एंटर केल्यानंतर नोडज, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) प्रथम स्थापित करण्याची शिफारस केली जाते आणि नंतर `direnv allow` (निर्देशिका प्रविष्ट केल्यानंतर [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वयंचलितपणे कार्यान्वित होईल).

अर्थ असा आहे: जपानी, कोरियन, इंग्रजी, इतर सर्व भाषांमध्ये चीनी भाषांतर. तुम्हाला फक्त चीनी आणि इंग्रजीचे समर्थन करायचे असल्यास, तुम्ही फक्त `zh: en` लिहू शकता.

अर्थ असा आहे: जपानी, कोरियन, इंग्रजी, इतर सर्व भाषांमध्ये चीनी भाषांतर. तुम्हाला फक्त चीनी आणि इंग्रजीचे समर्थन करायचे असल्यास, तुम्ही फक्त `zh: en` लिहू शकता.

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

### दस्तऐवज भाषांतर ऑटोमेशन सूचना

कोड रेपॉजिटरी [xxai-art/doc](https://github.com/xxai-art/doc) पहा

डिरेक्टरी एंटर केल्यानंतर नोडज, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) प्रथम स्थापित करण्याची शिफारस केली जाते आणि नंतर `direnv allow` (निर्देशिका प्रविष्ट केल्यानंतर [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वयंचलितपणे कार्यान्वित होईल).

शेकडो भाषांमध्ये अनुवादित झालेला मोठा कोड बेस टाळण्यासाठी, मी प्रत्येक भाषेसाठी स्वतंत्र कोड बेस तयार केला आणि कोड बेस साठवण्यासाठी एक संस्था तयार केली.

`GITHUB_ACCESS_TOKEN` पर्यावरण व्हेरिएबल सेट करणे आणि नंतर [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) चालवणे आपोआप कोड रेपॉजिटरी तयार करेल.

अर्थात, तुम्ही ते कोड बेसमध्ये देखील ठेवू शकता.

भाषांतर स्क्रिप्ट संदर्भ [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

स्क्रिप्ट कोडचा अर्थ खालीलप्रमाणे आहे:

[bunx](https://bun.sh/docs/cli/bunx) हे npx चे बदली आहे, जे जलद आहे. अर्थात, जर तुम्ही बन इंस्टॉल केलेले नसेल, तर तुम्ही त्याऐवजी `npx` वापरू शकता.

`bunx mdt zh` `.mdt` zh डिरेक्टरीमध्ये `.md` म्हणून रेंडर करते, खालील 2 लिंक केलेल्या फाइल्स पहा

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` हा अनुवादासाठी मुख्य कोड आहे (जर तुमच्याकडे फक्त `nodejs` स्थापित केले असतील, परंतु `bun` आणि `direnv` स्थापित केले नसेल, तर तुम्ही भाषांतर करण्यासाठी `npx i18n` देखील चालवू शकता).

हे [i18n.yml चे](https://github.com/xxai-art/doc/blob/main/i18n.yml) विश्लेषण करेल, या दस्तऐवजातील `i18n.yml` चे कॉन्फिगरेशन खालीलप्रमाणे आहे:

```
en:
zh: ja ko en
```

अर्थ असा आहे: जपानी, कोरियन, इंग्रजी, इतर सर्व भाषांमध्ये चीनी भाषांतर. तुम्हाला फक्त चीनी आणि इंग्रजीचे समर्थन करायचे असल्यास, तुम्ही फक्त `zh: en` लिहू शकता.

शेवटचे आहे [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , जे मुख्य शीर्षक आणि प्रत्येक भाषेच्या `README.md` च्या पहिल्या उपशीर्षकामधील सामग्री काढते आणि `README.md` एंट्री तयार करते. कोड अगदी सोपा आहे, तुम्ही तो स्वतः पाहू शकता.

Google API विनामूल्य भाषांतरासाठी वापरला जातो. तुम्ही Google मध्ये प्रवेश करू शकत नसल्यास, कृपया कॉन्फिगर करा आणि प्रॉक्सी सेट करा, जसे की:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

भाषांतर स्क्रिप्ट `.i18n` निर्देशिकेत अनुवादित कॅशे तयार करेल, कृपया ते `git status` तपासा आणि पुनरावृत्ती होणारे भाषांतर टाळण्यासाठी ते कोड रिपॉझिटरीमध्ये जोडा.

कृपया प्रत्येक वेळी कॅशे अपडेट करण्यासाठी भाषांतरात सुधारणा करताना `bunx i18n` चालवा.

मूळ मजकूर आणि भाषांतर एकाच वेळी सुधारित केले असल्यास, कॅशे गोंधळात पडेल, म्हणून जर तुम्हाला सुधारित करायचे असेल, तर तुम्ही फक्त एक सुधारित करू शकता आणि नंतर कॅशे अद्यतनित करण्यासाठी `bunx i18n` चालवा.
