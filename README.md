# engr-e511-assignment-4-solved
**TO GET THIS SOLUTION VISIT:** [ENGR-E511 Assignment 4 Solved](https://www.ankitcodinghub.com/product/engr-e511-assignment-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100334&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ENGR-E511 Assignment 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
P1: kNN Source Separation

<ol>
<li>Prepare your S and N matrices by using the procedure in Homework 3 P3.1. In addition to them, let’s create another matrix G, the magnitude spectrogram of trs.wav+trn.wav. Also, let’s create yet another matrix called Ideal Binary Masks (IBM), B defined in Homework 3 P3 (or repeatedly as follows):
􏰊1 ifSf,t≥Nf,t

Bf,t = 0 otherwise. (1)

MyhopeisthatS≈B⊙G. Thissoundsabittoorough,butyouknowitworkstosome degree as shown in Homework 3 P3.
</li>
<li>Load x nmf.wav and convert it into a complex-valued spectrogram X and its magnitudes Y , respectively. This time, we compare each column of Y with all columns in G to find out k nearest neighbors. Then, for t-th given test frame in Y we have a list of indices to the k nearest frames in G, e.g. {i1,i2,··· ,ik}, where i1,i2,··· ,ik ∈ {1,··· ,990}, where 990 is the number of frames in G (yours can be slightly different depending on the STFT setup). For the comparison, I used Euclidean distance for no good reason, but you can choose a different (more proper) one if you want.</li>
<li>What we want to do with this kNN search is to predict the unknown IBM of the test signal, D ∈ B513×131 (again 131 is the number of frames in Y ). By using the nearest neighbor indices, I can collect the IBM vectors from B, i.e. {B:,i1 , B:,i2 , · · · , B:,ik }. Since Y :,t is very similar
1
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
to {G:,i1,G:,i2,··· ,G:,ik}, I hope that my D:,t should be similar to {B:,i1,B:,i2,··· ,B:,ik}. How do we consolidate them though? Let’s try median of them, because that’ll give you one if one is the majority, and vice versa:

D:,t = median({B:,i1 , B:,i2 , · · · , B:,ik }). (2)

4. Repeat this for all your test frames (131 frames in my STFT) and predict the full D matrix. Recover the complex-valued spectrogram of your speech by masking the input: Sˆtest = D⊙X. Convert it back to the time domain. Listen to it. Is the noise suppressed? Submit this wavefile as well as your code.

P2: Motor Imagery

<ol>
<li>eeg.mat has the training and testing samples as well as their labels. Use them to replicate my BCI classification experiments in Module 5 (not the entire lecture, but from S3 to S8 and S37). But, instead of PCA dimension reduction, we’re going to use locality sensitive hashing to extract binary features. Also, instead of na ̈ıve Bayes, we’ll do kNN classification.</li>
<li>For the kNN classification, for every test example you have to find the K nearest neighbors from 112 training samples. You’re lucky. This kNN search is not a big deal, because your training set is tiny. However, as your professor I have to help you guys be prepared for your future big data projects at your fancy new job after your graduation (don’t forget me). So, I’m giving you this homework assignment that will help you come up with a speed-up technique for the kNN search. It’s not that complicated.</li>
<li>Come up with a random projection matrix A ∈ RL×M, where M denotes the number of dimensions of your data samples (5 rows of your magnitude STFT, vectorized), 2551, and L is the new dimension after this random projection. So, you’re replacing PCA with this random projection. Note that L doesn’t always have to be smaller than M. Although A is a matrix with random values, you should make sure that the row vectors (the projection vectors) should be unit vectors, i.e. ||Ai,:||2 = 1. Make sure of it.</li>
<li>Do the random projection and take the sign of the result (element-wise), so that your random projection produces a bunch of +1’s and -1’s:
Y = sign(AX1:M,:) (3)
</li>
<li>Use this A matrix and the sign function wrapper to convert your 255 dimensional TRAINING samples into L-dimensional bipolar binary hash codes. Ditto for the TEST samples (use the same A matrix). If you’re not comfortable with bipolar binaries, you can turn them into 0-1 binaries by replacing -1’s with 0’s. It’s up to you.</li>
<li>Do your kNN classification using these binary version of your data samples. Note that you can compare the test bit string with the bit strings of the training data by using the Hamming distance, instead of the Eucleadian distance between the original real-valued vectors. You know your computer prefers binary values, right? This way you can speed up the comparison,</li>
</ol>
1Note that this number comes from the calculation [# channels] × [# frames] × [# subbands], while # frames can slightly vary depending on your STFT implementation. Mine resulted in 3 × 17 × 5 = 255

2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
and eventually the kNN search (although you might not be able to see the actual speed-up due to the too small dataset size and your script language that doesn’t exploit binary variables). Report your classification results with different choice of K and L. I think a table of accuracies will be great. You don’t have to submit all the intermediate plots. What I need to see is the accuracies and your source code.

7. Compare your results with mine in M5 S37. You’re classifier is based on binary variables and bitwise operations, so you must have expected a big performance drop. How do you like it eventually? Report your classification accuracy. Submit your code and your discussion.

P3: Multidimensional Scaling

1. MDS pdist.mat holds a 996×996 square matrix, which holds squared pairwise Euclidean dis- tances that I constructed from a set of data points. Of course I won’t share the original data samples with you. Instead, you’ll write a multidimensional scaling code for this so that you can recover the original map out of L. If your MDS routine is successful, you should be able to see what the original map was. The original map was in the 2D space, so you may want to see two largest eigenvectors. Report the map you recovered in the form of a scatter plot.

2. Note that the MDS result can be rotated and shifted.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
