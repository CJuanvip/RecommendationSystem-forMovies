Implementing in progress:

Real-life optimization(reduce complexity using map-reduce)
https://hal.archives-ouvertes.fr/hal-01406473/file/final.pdf


Combination of LDA with Collaborative filtering:
https://www.researchgate.net/publication/305415848_Rating_LDA_Model_for_Collaborative_Filtering

Some scholars apply LDA to review texts to obtain additional information for recommendation systems. For example, McAuley and Leskovec first mined user interests from product reviews by using LDA and then combined matrix factorization to predict the unknown item ratings. Wilson et al utilized LDA to infer the latent properties of items from their textual descriptions and then calculated users’ preferences or persona in the same latent topic space based on historical ratings. However, these methods rely on additional text information and can not be applied to the situation without text data. Others used LDA for collaborative filtering directly. For example, Liu et al achieved the proposed enhancing of collaborative filtering by using the LDA to mine user interests. Zhao et al used LDA to learn the probability that a user rates an item. These methods can be easily applied to collaborative filtering.

What I plan to implement:

A probabilistic latent interest model.
To consider the impact of ratings when a consumer selects an item,
we incorporate rating information into the LDA model. A user’s
choice is not only influenced by his/her interests, but also by the
ratings of others. The key idea of the RLDA model assumes that,
under similar interest, the higher the proportion of high ratings,
the more popular the items.

Compared with previous works, the main difference of our
model is our model views the ratings and items not separately, but
as a whole, resulting in not only retaining rating information, but
also reducing the calculation steps. 

In particular, the proposed algorithm can not only predict the unknown item ratings, but also
get user’s interest distribution. It is worth noting that the model
views the recommendation problem as a ranking problem.








* recsys_ui: html5+JavaScript+jquery+ajax
* recsys_web: Java+SpringBoot+mysql
* recsys_spider: Python+BeautifulSoup+Selenium
* recsys_sql: SQL
* recsys_model: libFM, sklearn. 


Content-base + LibFM + RL + LR

Link to related reference:

LDA theory: https://zhuanlan.zhihu.com/p/31470216

Optimize Recommendation: https://towardsdatascience.com/4-ways-to-supercharge-your-recommendation-system-aeac34678ce9

General Recommendation: https://github.com/nikbearbrown/INFO_6105/blob/925e7e6b7ee3e547e8b87c3dfb053d2546e3c634/Recommender_Systems/Recommender_Systems.ipynb

FM advantages: https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf. /. https://zhuanlan.zhihu.com/p/50426292
