---
title: "The Moral Choice Machine"
collection: publications
permalink: /publication/2020-05-20-moral-choice-machine
excerpt: 'todo.'
date: 2020-05-20
venue: 'Frontiers in Artificial Intelligence'
paperurl: 'https://www.frontiersin.org/articles/10.3389/frai.2020.00036/pdf'
citation: 'Schramowski, P., Turan, C., Jentzsch, S., Rothkopf, C., & Kersting, K.. (2010). &quot;The moral choice machine.&quot; <i>Frontiers in Artificial Intelligence</i>. 3, 36.'
---
Allowing machines to choose whether to kill humans would be devastating for world peace and security. But how do we equip machines with the ability to learn ethical or even moral choices? In this study, we show that applying machine learning to human texts can extract deontological ethical reasoning about “right” and “wrong” conduct. We create a template list of prompts and responses, such as “Should I [action]?”, “Is it okay to [action]?”, etc. with corresponding answers of “Yes/no, I should (not).” and "Yes/no, it is (not)." The model's bias score is the difference between the model's score of the positive response (“Yes, I should”) and that of the negative response (“No, I should not”). For a given choice, the model's overall bias score is the mean of the bias scores of all question/answer templates paired with that choice. Specifically, the resulting model, called the Moral Choice Machine (MCM), calculates the bias score on a sentence level using embeddings of the Universal Sentence Encoder since the moral value of an action to be taken depends on its context. It is objectionable to kill living beings, but it is fine to kill time. It is essential to eat, yet one might not eat dirt. It is important to spread information, yet one should not spread misinformation. Our results indicate that text corpora contain recoverable and accurate imprints of our social, ethical and moral choices, even with context information. Actually, training the Moral Choice Machine on different temporal news and book corpora from the year 1510 to 2008/2009 demonstrate the evolution of moral and ethical choices over different time periods for both atomic actions and actions with context information. By training it on different cultural sources such as the Bible and the constitution of different countries, the dynamics of moral choices in culture, including technology are revealed. That is the fact that moral biases can be extracted, quantified, tracked, and compared across cultures and over time.

[Download paper here](https://www.frontiersin.org/articles/10.3389/frai.2020.00036/pdf)

Recommended citation: Schramowski, P., Turan, C., Jentzsch, S., Rothkopf, C., & Kersting, K. (2020). "The moral choice machine." <i>Frontiers in Artificial Intelligence, 3, 36</i>.