> चित्र [Dmitry Soshnikov](http://soshnikov.com) द्वारा

जैसे-जैसे समय बीतता गया, कंप्यूटिंग संसाधन सस्ते होते गए, और अधिक डेटा उपलब्ध होने लगा, इसलिए न्यूरल नेटवर्क के दृष्टिकोण ने कई क्षेत्रों में मानवों के साथ प्रतिस्पर्धा में उत्कृष्ट प्रदर्शन दिखाना शुरू कर दिया, जैसे कि कंप्यूटर दृष्टि या भाषण समझना। पिछले दशक में, कृत्रिम बुद्धिमत्ता (Artificial Intelligence) शब्द का उपयोग ज्यादातर न्यूरल नेटवर्क के पर्याय के रूप में किया गया है, क्योंकि जो भी AI सफलताएँ हम सुनते हैं, वे अधिकांशतः इन पर आधारित होती हैं।

हम देख सकते हैं कि दृष्टिकोण कैसे बदले हैं, उदाहरण के लिए, एक शतरंज खेलने वाले कंप्यूटर प्रोग्राम बनाने में:

* प्रारंभिक शतरंज कार्यक्रम खोज पर आधारित थे - एक कार्यक्रम स्पष्ट रूप से अगले कुछ चालों के लिए एक प्रतिकारी के संभावित चालों का अनुमान लगाने की कोशिश करता था, और कुछ चालों में प्राप्त होने वाली सर्वोत्तम स्थिति के आधार पर एक सर्वोत्तम चाल का चयन करता था। यह [alpha-beta pruning](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning) खोज एल्गोरिदम के विकास की ओर ले गया।
* खोज रणनीतियाँ खेल के अंत की ओर अच्छी तरह से काम करती हैं, जहाँ खोज स्थान संभावित चालों की एक छोटी संख्या द्वारा सीमित होती है। हालाँकि, खेल की शुरुआत में, खोज स्थान विशाल होता है, और एल्गोरिदम को मानव खिलाड़ियों के बीच मौजूदा मैचों से सीखकर सुधारा जा सकता है। बाद के प्रयोगों में [case-based reasoning](https://en.wikipedia.org/wiki/Case-based_reasoning) का उपयोग किया गया, जहाँ कार्यक्रम खेल में वर्तमान स्थिति के समान ज्ञान आधार में मामलों की खोज करता था।
* आधुनिक कार्यक्रम जो मानव खिलाड़ियों पर जीत हासिल करते हैं, वे न्यूरल नेटवर्क और [reinforcement learning](https://en.wikipedia.org/wiki/Reinforcement_learning) पर आधारित होते हैं, जहाँ कार्यक्रम केवल अपने आप से खेलकर और अपनी गलतियों से सीखकर खेलने का तरीका सीखते हैं - जैसे कि मानव शतरंज खेलने में सीखते हैं। हालाँकि, एक कंप्यूटर कार्यक्रम बहुत कम समय में कई अधिक खेल खेल सकता है, और इस प्रकार बहुत तेजी से सीख सकता है।

✅ अन्य खेलों पर थोड़ा शोध करें जो AI द्वारा खेले गए हैं।

इसी तरह, हम देख सकते हैं कि "बात करने वाले कार्यक्रमों" (जो ट्यूरिंग टेस्ट पास कर सकते हैं) बनाने के दृष्टिकोण में कैसे बदलाव आया है:

* इस प्रकार के प्रारंभिक कार्यक्रम जैसे [Eliza](https://en.wikipedia.org/wiki/ELIZA), बहुत सरल व्याकरणिक नियमों और इनपुट वाक्य को प्रश्न में पुनः-फार्मेट करने पर आधारित थे।
* आधुनिक सहायक, जैसे Cortana, Siri या Google Assistant सभी हाइब्रिड सिस्टम हैं जो भाषण को पाठ में परिवर्तित करने और हमारी मंशा को पहचानने के लिए न्यूरल नेटवर्क का उपयोग करते हैं, और फिर आवश्यक क्रियाएँ करने के लिए कुछ तर्क या स्पष्ट एल्गोरिदम का उपयोग करते हैं।
* भविष्य में, हम एक पूर्ण न्यूरल-आधारित मॉडल की उम्मीद कर सकते हैं जो संवाद को स्वयं संभाल सके। हाल के GPT और [Turing-NLG](https://turing.microsoft.com/) न्यूरल नेटवर्क के परिवार ने इस मामले में शानदार सफलता दिखाई है।

> चित्र [Dmitry Soshnikov](http://soshnikov.com), [फोटो](https://unsplash.com/photos/r8LmVbUKgns) [Marina Abrosimova](https://unsplash.com/@abrosimova_marina_foto) द्वारा, Unsplash

## हाल के AI अनुसंधान

न्यूरल नेटवर्क अनुसंधान में हालिया विशाल वृद्धि 2010 के आसपास शुरू हुई, जब बड़े सार्वजनिक डेटासेट उपलब्ध होने लगे। एक विशाल छवियों का संग्रह जिसे [ImageNet](https://en.wikipedia.org/wiki/ImageNet) कहा जाता है, जिसमें लगभग 14 मिलियन एनोटेटेड छवियाँ हैं, ने [ImageNet Large Scale Visual Recognition Challenge](https://image-net.org/challenges/LSVRC/) को जन्म दिया।

![ILSVRC Accuracy](../../../../lessons/1-Intro/images/ilsvrc.gif)

> चित्र [Dmitry Soshnikov](http://soshnikov.com) द्वारा
In 2012, [Convolutional Neural Networks](../4-ComputerVision/07-ConvNets/README.md) का पहली बार छवि वर्गीकरण में उपयोग किया गया, जिससे वर्गीकरण त्रुटियों में एक महत्वपूर्ण कमी आई (लगभग 30% से 16.4% तक)। 2015 में, Microsoft Research का ResNet आर्किटेक्चर [मानव-स्तरीय सटीकता](https://doi.org/10.1109/ICCV.2015.123) प्राप्त करने में सफल रहा।

तब से, न्यूरल नेटवर्क ने कई कार्यों में बहुत सफल व्यवहार प्रदर्शित किया है:

---

वर्ष | मानव समानता प्राप्त की
-----|--------
2015 | [छवि वर्गीकरण](https://doi.org/10.1109/ICCV.2015.123)
2016 | [संवादात्मक भाषण पहचान](https://arxiv.org/abs/1610.05256)
2018 | [स्वचालित मशीन अनुवाद](https://arxiv.org/abs/1803.05567) (चीनी से अंग्रेजी)
2020 | [छवि कैप्शनिंग](https://arxiv.org/abs/2009.13682)

पिछले कुछ वर्षों में, हमने बड़े भाषा मॉडलों, जैसे कि BERT और GPT-3 के साथ विशाल सफलताओं का गवाह बने हैं। यह मुख्य रूप से इस तथ्य के कारण हुआ कि बहुत सारे सामान्य पाठ डेटा उपलब्ध हैं जो हमें मॉडलों को पाठों की संरचना और अर्थ को कैप्चर करने के लिए प्रशिक्षित करने की अनुमति देते हैं, उन्हें सामान्य पाठ संग्रह पर पूर्व-प्रशिक्षित करते हैं, और फिर उन मॉडलों को अधिक विशिष्ट कार्यों के लिए विशेषीकृत करते हैं। हम इस पाठ्यक्रम में बाद में [प्राकृतिक भाषा प्रसंस्करण](../5-NLP/README.md) के बारे में और अधिक जानेंगे।

## 🚀 चुनौती

इंटरनेट का दौरा करें ताकि यह निर्धारित किया जा सके कि आपके अनुसार, एआई का सबसे प्रभावी उपयोग कहाँ किया जा रहा है। क्या यह एक मैपिंग ऐप में है, या किसी भाषण-से-टेक्स्ट सेवा में या एक वीडियो गेम में? शोध करें कि सिस्टम कैसे बनाया गया था।

## [व्याख्यान के बाद का प्रश्नोत्तरी](https://red-field-0a6ddfd03.1.azurestaticapps.net/quiz/201)

## समीक्षा और आत्म अध्ययन

[इस पाठ](https://github.com/microsoft/ML-For-Beginners/tree/main/1-Introduction/2-history-of-ML) के माध्यम से एआई और एमएल के इतिहास की समीक्षा करें। उस पाठ या इस पाठ के शीर्ष पर स्केच नोट से एक तत्व लें और इसके विकास को सूचित करने वाले सांस्कृतिक संदर्भ को समझने के लिए इसे अधिक गहराई से शोध करें।

**कार्य**: [गेम जाम](assignment.md)

**अस्वीकृति**:  
यह दस्तावेज़ मशीन-आधारित एआई अनुवाद सेवाओं का उपयोग करके अनुवादित किया गया है। जबकि हम सटीकता के लिए प्रयासरत हैं, कृपया ध्यान दें कि स्वचालित अनुवाद में त्रुटियाँ या गलतियाँ हो सकती हैं। मूल दस्तावेज़ को उसकी मूल भाषा में अधिकारिक स्रोत माना जाना चाहिए। महत्वपूर्ण जानकारी के लिए, पेशेवर मानव अनुवाद की सिफारिश की जाती है। इस अनुवाद के उपयोग से उत्पन्न किसी भी गलतफहमी या गलत व्याख्या के लिए हम जिम्मेदार नहीं हैं।