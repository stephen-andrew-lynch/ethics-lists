# An Ethics-List Update

This started as an attempt to keep an up-to-date list of all of the AI ethics-related resources on the web, but fell by the wayside when I left LinkedIn to pursue other professional interests in late 2021. I am going to make a second go at updating the list in early 2025. 

***

# 2021 "Understanding Responsible AI" Note

I created a primer email about "understanding responsible AI 101" note that I typically sent to journalists starting in 2019 and got tons of positive feeback from folks who were grokking what was new and happening in the field. I eventually published a public version on LinkedIn in 2021. You can see the full post on LinkedIn [here](https://www.linkedin.com/pulse/fast-easy-comprehensive-introduction-responsible-ai-us-stephen-lynch/?trackingId=q6rw6rVzQySLpSY1L4ymJQ%3D%3D).

I've also recreated the post below, for your reading pleasure. 

## A Fast, Easy & Comprehensive introduction to Responsible AI for us nontechnical folks (j/k, you can only choose two)
By Stephen Lynch
August 17, 2021

I've spent five years working with the LinkedIn Engineering Data org, and for all five of those years I've been privileged to sit in on conversations about what can broadly be termed responsible AI or (when discussed more broadly) responsible design; making sure our use of data and AI first avoid causing harm and second are used to make the world a more fair place. 

Explaining this topic to other Comms professionals or reporters is complicated, owing to the fact that talking about AI can itself be complicated… and then you're adding on top of it a discussion of LinkedIn's products, general notions of fairness/equity, discussions of intersectional harms, academic research in the field, etc. It's all really complicated!

In order to help interested folks bootstrap their understanding of fairness in AI, there's an email I've developed over the years that gives a quick overview of some of the AI fairness "greatest hits" in a format that lets you first skim my (very cursory) summaries, and then dig in where you're interested. 

*Disclaimer: I am not a responsible AI expert. I am just informed enough to write an article like this, but definitely ignorant enough to omit some key research and concepts. Please do not rely on me as your sole source of information on this subject!*

But first (because I am a PR person after all), here's a quick survey of some of the work that's happened here at LinkedIn in this field:

- ["An Update on LinkedIn's Actions Towards Equity"](https://www.linkedin.com/pulse/update-linkedins-actions-towards-equity-imani-dunbar/): This post isn't technically about AI, but truly "responsible AI" is arguably as much about the setting that an AI-powered product or service is deployed in as the algorithms or training data that are used (cf. Keyes et al, below). We have done several updates that focus on new product changes, unrelated to AI, that have a huge impact on how these products impact peoples lives (as recently as (last week)[https://www.linkedin.com/business/talent/blog/product-tips/source-and-build-more-diverse-talent-pools?lipi=urn%3Ali%3Apage%3Ad_flagship3_pulse_read%3B%2FFN21vGRSXGbuboPJ4IWFQ%3D%3D]!). 

- ["Addressing bias in large-scale AI applications: The LinkedIn Fairness Toolkit"](https://www.linkedin.com/blog/engineering/fairness/lift-addressing-bias-in-large-scale-ai-applications) & ["Bringing Project Every Member to life: Open sourcing our Spark inequality A/B testing library"](https://www.linkedin.com/blog/engineering/member-customer-experience/bringing-project-every-member-to-life) (both 2020): One of our recent, major open source projects that allows any other company to replicate the process of measuring intent & impact of not just their own AI systems, but any product, generally. We can say that these approaches work, because we have receipts. 

- ["The Case for Responsible AI Design"](https://www.linkedin.com/blog/engineering/fairness/fairness-privacy-transparency-by-design) (2020): In another post, Chief Data Officer Igor Perisic lays out the challenges facing the AI field and discusses how our approach is naturally aligned with the OECD's position paper on AI. 

- ["Fairness, Privacy, and Transparency by Design in AI/ML Systems"](https://www.linkedin.com/blog/engineering/fairness/fairness-privacy-transparency-by-design) (2019): An embarrassment of riches for researchers. I am still not sure if any of the reporters that I have sent this to have ever read the entire thing. :) 

- ["Building Representative Talent Search at LinkedIn"](https://www.linkedin.com/blog/engineering/hiring/building-representative-talent-search-at-linkedin) (2018): In 2018, LinkedIn took the big jump of revamping the core search AI for our core product for our core business to focus on inclusion and fairness. It's incredible to think that this work is now three years old. 

- ["Making Hard Choices: The Quest for Ethics in Machine Learning"](https://www.linkedin.com/blog/engineering/archive/making-hard-choices-the-quest-for-ethics-in-machine-learning) (2016): One of the earliest public statements that I can recall coming from a senior leader in the tech industry about responsible AI and machine learning (although obviously many researchers were discussing this earlier).

Let's dive in to some essential academic reading and primary sources:

First up, here are some of the relatively famous papers and studies in the field, all of which are worth taking the time to read in full, when you're ready.

- Buolamwini & Gebru (2017-2018)--Gender Shades study: What (should be) one of the widely-known examples of algorithmic bias used in production systems. Watching talks by Joy Buolamwini and Timnit Gebru about how facial recognition systems got to the point where they were much worse at identifying the faces of black women is also very illuminating WRT topics of AI fairness in general. [gendershades.org](http://gendershades.org/)

- Crawford & Calo (2016)--"There is a blind spot in AI research": Evaluating AI outside of its social context may seem like a simple idea, but it was one that was sorely lacking from the discussion of responsible AI prior to 2016: [Nature](https://www.nature.com/articles/538311a)

- Angwin, Larson, Mattu & Kirchner, ProPublica's "Machine Bias" (2016) analysis of the COMPAS sentencing algorithm: Conversations about fairness in AI are inextricably linked to the way they're used in the real world, and this is an example of systemic problems in a much higher-stakes domain than 99.9% of AI systems: [ProPublica](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)

- Karen Hao, MIT Technology Review (2019)--"This is how AI bias really happens—and why it's so hard to fix": The shortest and perhaps most comprehensive explanation of the different considerations that need to be discussed (and they all need to be discussed) when you're discussing issues of algorithmic bias. [MIT Technology Review](https://www.technologyreview.com/2019/02/04/137602/this-is-how-ai-bias-really-happensand-why-its-so-hard-to-fix/)

There are also lots of very accessible papers that discuss the ways that many of problems in fairness, AI bias, etc. are products of some fundamental assumptions that have been made by computer scientists (rather than outright nefarious motives or willful negligence).

- Lipton & Steinheart (2018)--Troubling Trends in Machine Learning Scholarship: A very engaging description of some of the problems in the AI community. The section on "suitcase words" is probably required reading for any PR person or reporter who is interested in this subject (and something I grappled with in writing this post :)). [arXiv](https://arxiv.org/pdf/1807.03341.pdf)

- Hutchinson & Mitchell--50 Years of Test (Un)fairness: Lessons for Machine Learning: Another great, very readable survey of AI fairness issues. I also heartily recommend watching or listening to any talk by Margaret Mitchell, if you find this subject to be interesting. [m-mitchell.com](http://www.m-mitchell.com/papers/History_of_Fairness-arxiv.pdf)

- Gebru, Wallach & Crawford--Datasheets for Datasets: There are lots of problems in AI, but what about solutions? Some of them aren't based on algorithms at all. Much like some of LinkedIn's internal efforts, Gebru et al recommend including better & more meaningful metadata on AI training datasets. [arXiv](https://arxiv.org/pdf/1803.09010.pdf)

- Hardt, Price & Srebro--Equality of Opportunity in Supervised Learning/Pratik Gajane & Mykola Pechenizkiy--On Formalizing Fairness in Prediction with Machine Learning: What does "fair" even mean? It turns out that it can mean different things in different contexts, and if you want an AI system to be fair… then you really need to define it well. [NIPS](http://papers.nips.cc/paper/6374-equality-of-opportunity-in-supervised-learning.pdf) && [arXiv](https://arxiv.org/pdf/1710.03184.pdf)

- Keyes, Hutson & Durbin--A Mulching Proposal: A cautionary tale for anyone who thinks AI fairness can be treated as a PR or purely academic exercise; A Modest Proposal for the ICML set. [ironholds.org](https://ironholds.org/resources/papers/mulching.pdf)

Next, here are some non-academic reports/projects on applications of responsible AI in policy and the real world implications of some of these technologies:

- European Commission--The Age of Artificial Intelligence Towards a European Strategy for Human-Centric Machines: [ec.europa.eu](https://ec.europa.eu/epsc/sites/epsc/files/epsc_strategicnote_ai.pdf)

- White House--Big Data: A Report on Algorithmic Systems, Opportunity, and Civil Rights: [obamawhitehouse.archives.gov](https://obamawhitehouse.archives.gov/sites/default/files/microsites/ostp/2016_0504_data_discrimination.pdf)

- RAND--"Pitfalls of Predictive Policing": [rand.org](https://www.rand.org/blog/2016/10/pitfalls-of-predictive-policing.html)

Finally, if you've read this far, check out this talk by our own Guillaume Saint-Jacques talking about key considerations in responsible AI research at LinkedIn:

**HBS Digital Initiative:**[Approaches to Fairness, Equity, and Inequality at LinkedIn | Guillaume Saint-Jacques](https://www.youtube.com/watch?v=Br0GfSnzUsU)
