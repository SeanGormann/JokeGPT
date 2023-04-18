# JokeGPT
Building a transformer architecture from scratch.

This project was all about understanding the transformer architechture - the data preprocessing necessary, tokenization, multiheaded attention, self attention and more. It was great to get a thorough understanding of these topics, and I look forward to exploring them further. For this project I mainly followed the tutorial presented by Andrej Karpathy which can be found: [Here](https://www.youtube.com/watch?v=kCc8FmEb1nY&t=465s&ab_channel=AndrejKarpathy) 

I thought it would be fun to train the transformer on a dataset full of jokes, hence the name JokeGPT (or JPT). Some light preparation and data cleaning was carried out in the just-jokes notebook, but again, the main focus of this project was understanding what's under the hood of transformers. After a simple epoch of training on this data, the decoded output is essentially gibberish:

---

*dkqehbaihSD AdknsfSADXkwj!inwoen*

*wdciwnndibwnbcxSKCNwandADNiWndANan??SCDNSOD??*

*wsWDCWD>wdjkb???Swdm??adW*

---

The model was just shy of 11 million parameters, which is no small feat to train. I used google colab and it's copious amount of GPU resources for training. After about 10,000 epochs, the outputs began to become somewhat recognisable:

---

*What do you call a deer with no eyes? No eye-deer What do you call a redneck with no eyes? No-eye-deer What do you call a deer with no legs? Deer balls. What do you call a deer with no legs? Deer - Goodbye. Why don't you always have any legs?*

*What did the pirate girl say to her favorite drink? You don't carve*

*Why were the spaghetto players good at Halloween Jersey's Detroit? Because no one can wash her car with anything.*

*why is a donut like an attractic letter? It hasn't cared a condom.*

---

Now don't get my wrong, it's still mostly gibberish. However, it's striking how closely the output is starting to resemble the training data. With larger data sets and optimal tokenization methods one can easily see how these models perform so impressively in generating text.
