---
tags: tip
title: धत तेरे की, मुझे 5 commits से पहले की commit को पूर्ववत करने की जरूरत है!
id: undo-a-commit
order: 7
---

```git
# आप पूर्ववत करने के लिए commit खोजे
git log
# इतिहास में ऊपर और नीचे स्क्रॉल करने के लिए तीर कुंजियों का उपयोग करें
# एक बार जब आप अपना commit पा लेते हैं, तो हैश सेव करें
git revert [saved hash]
# git एक नया commit बनाएगा जो की उस commit को पूर्ववत करता है
# संकेतों का पालन करते हुए commit सन्देश को ठीक करें 
# या बस सेव और commit करें
```

परिवर्तनों को पूर्ववत करने के लिए आपको पुरानी फ़ाइल सामग्री को खोजने और कॉपी-पेस्ट करने की आवश्यकता नहीं है! यदि आपने कोई बग commit किया है, तो आप `revert` के साथ एक बार में सभी कमिट को पूर्ववत कर सकते हैं।

आप एक पूर्ण commit के बजाय किसी एकल फ़ाइल को वापस भी ला सकते हैं! लेकिन निश्चित रूप से, सच्चे Git फैशन में, यह एक पूरी तरह से अलग आदेश होंगे ...