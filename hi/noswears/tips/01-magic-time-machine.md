---
tags: tip
title: धत तेरे की, मैंने कुछ बहुत गलत कर दिया है, कृपया मुझे बताएं कि Git में एक जादुई समय यंत्र है?!
id: magic-time-machine
order: 1
---

```git
git reflog
# आपको आपके पास मौजूद हर चीज की एक सूची दिखाई देगी
# जो आपने git में सभी branches में commit किया है!
# हर एक का एक इंडेक्स HEAD@{index} है
# उस commit का पता लगाएं, जहां से आपने गड़बड़ी शुरू की है
git reset HEAD@{index}
# जादुई समय यंत्र
```

आप इसके द्वारा गलती से हटाए गए किसी काम को वापस पा सकते हैं, या आपके द्वारा आजमाए गए किसी चीज़ को हटाने के लिए, या repository से गड़बड़ कोड हटाने के लिए, या खराब merge को ठीक करने के लिए, या फिर बस उस commit तक वापस जाने के लिए उपयोग कर सकते हैं जहां चीजें वास्तव में काम कर रही थी। मैं `reflog` का बहुत उपयोग करता हूँ। कई लोगों ने मुझे इसे जोड़ने का सुझाव दिया था, उनको मेरा सलाम!