
### Multi Modal Search

Resources for incorporating image embeddings, joint image/word embeddings, multi lingual word embeddings for learning to rank or as a replacement for things like BM25 or TFIDF.

1. Kamelia Aryafar (Overstock, formerly Etsy)
Learning to Rank in Ecommerce AIWTB 2017
https://arxiv.org/abs/1511.06746 (Nov 2015)
https://www.youtube.com/watch?v=QjTi1qcLTQw

* In production retrieve top k documents using SOLR and bm25.  Then rerank the the returned results.
Concatenation of transfer learned image embeddings from a VGG model trained on ImageNet with bag of words
Learning rank from search logs using click and ignore signals

* Great examples of overcoming user labels for Wedding dresses that are not relevant.


2. Ethan Rosenthal (Dia & Co, Birchbox)  
Ethan writes very accessible content and prefers methods that are intuitive.
* He obtained great results from transfer learning on ImageNet VGG model after expending significant effort trying to incorporate side channel information using matrix factorization methods ( WRMF weighted regularized matrix factorization )

* Diving into the deep end of clothing styles  
 https://www.youtube.com/watch?v=Pm4ZQMKoz7Q  
 http://blog.ethanrosenthal.com/  
 http://blog.ethanrosenthal.com/2017/06/20/matrix-factorization-in-pytorch/  
 https://github.com/EthanRosenthal  

* Slide presentation links from Ethan  
https://www.slideshare.net/rosentep/diving-into-the-deep-end-of-clothing-styles-pydata-nyc-2017  
https://www.slideshare.net/CalvinGiles/finding-needles-in-haystacks-with-deep-neural-networks  
https://www.slideshare.net/AhmadQamar3/using-deep-neural-networks-for-fashion-applications  
https://medium.com/mlreview/how-to-apply-distance-metric-learning-for-street-to-shop-problem-d21247723d2a  

3. Ivona Tautkute  
* good use case Ikea furniture
* Ikea would have structured data to use as labels for images
* What looks good with my sofa?  
https://www.youtube.com/watch?v=lA9swUze2kg  
https://arxiv.org/abs/1707.06907  
https://github.com/ivonatau  

4. Han Xiao (Zalando)  
Building Cross-Lingual End-to-End Product Search with Tensorflow  
https://hanxiao.github.io/2018/01/10/Build-Cross-Lingual-End-to-End-Product-Search-using-Tensorflow/  

5. Babylonpartners / fastText_multilingual  
alignment of multiple fastText word embeddings into a single vector space  
https://github.com/Babylonpartners/fastText_multilingual  

6. Aleksander Movchan  
* He assumes that you are already are familiar with "triplet loss functions"
* Triplet loss functions use an anchor, positive example, and a negative example
* You choose anchor, negative example pairs that are more similar to speed up training
* identifying a fashion item in a user image and finding it in an online shop  
https://medium.com/mlreview/how-to-apply-distance-metric-learning-for-street-to-shop-problem-d21247723d2a
* Florian Schoff 2015 Facenet paper that explains how to train models that use Triplet loss functions  
https://arxiv.org/abs/1503.03832

7. Shutterstock  
Great examples of overcoming disambiguation due to stemming.  
hawk -> some 'Stephen Hawking' along with 'hawk' that is a bird.  
angel -> 'Los Angeles' more than angel  
https://tech.shutterstock.com/2017/03/08/image-search-using-joint-embeddings-part-one/  
https://tech.shutterstock.com/2017/04/13/image-search-using-joint-embeddings-part-two/  

8.  Lyse clothing search blog post  
https://making.lyst.com/2018/01/10/a-machine-learning-model-to-understand-fashion-search-queries/  

9. Deep Fashion  
http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html

10. Dan Gillick (Google NLP group, instructor at Berkeley)  
Student talk at Berkeley
* learning embeddings in the same vector space for more than one media type
multi lingual search
* Increasing relevancy by returning more results from tail of documents.
* They mostly use Google search logs  
https://www.youtube.com/watch?v=JGHVJXP9NHw

11. Google AutoML announcment  
Use cases that are mostly about learning product attributes
https://www.blog.google/topics/google-cloud/cloud-automl-making-ai-accessible-every-business/
