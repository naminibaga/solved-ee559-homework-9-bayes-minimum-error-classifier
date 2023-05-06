Download Link: https://assignmentchef.com/product/solved-ee559-homework-9-bayes-minimum-error-classifier
<br>



<ol>

 <li>In this problem, consider a Bayes minimum-error classifier. Three classes are described by normal densities as follows:</li>

</ol>

<em>p</em>(<em>x S<sub>i </sub></em>)=   <em>N</em>(<em><u>x</u></em>,<em><u>m</u><sub>i</sub></em>,<u><sup>Σ</sup></u><em><sub>i </sub></em>),   <em>i </em>=1, 2, 3 <em>P</em>(<em>S</em><sub>1</sub>)=π<sub>1</sub>, <em>P</em>(<em>S</em><sub>2</sub>)=π<sub>2</sub>, <em>P</em>(<em>S</em><sub>3</sub>)=π<sub>3</sub>

in which each π<em><sub>i</sub></em> is a variable denoting the prior for class <em>S<sub>i</sub></em> (to save on writing).  Assume the π<em><sub>i</sub></em> are given.

In this problem, the algebra should be done by hand.  The plots may be done using computer or by hand.

<ul>

 <li>Write an expression for the discriminant functions <em>g<sub>i </sub></em>(<em><u>x</u></em>) , in two forms:

  <ul>

   <li>Expressed in terms of Mahalanobis distance <em>d<sub>M </sub></em>(<em><u>x</u></em>,<em><u>m</u><sub>i </sub></em>) and other given terms;</li>

   <li>Expressed only in terms of <em><u>x</u></em>, <em><u>m</u><sub>i</sub></em>, <u><sup>Σ</sup></u><em><sub>i</sub></em>, and <u><sup>Σ</sup></u><em><sub>i</sub></em><sup>−1</sup>, grouped as follows:</li>

  </ul></li>

</ul>

<em>g</em><em>i </em>(<em><u>x</u></em>)=<em><u>x</u></em><em>T<u>W </u></em><em>i <u>x</u></em>+<em><u>w</u></em><em>i <u>x</u></em>+<em>w</em>0(<em>i</em>)

and give expressions for <em><u>W</u></em>, <em><u>w</u></em>, and <em>w</em><sub>0</sub> in terms of the same quantities.

<ul>

 <li>State the decision rule in terms of the discriminant functions <em>g<sub>i </sub></em>(<em><u>x</u></em>). Is the classifier linear, quadratic, or neither? (c) For this part you are also given:</li>

</ul>

<em><u>m</u></em><sub>1</sub>=⎢⎡   <sup>1</sup><sub>2 </sub>⎤⎥⎦ ,   <em><u>m</u></em><sub>2 </sub>=⎡⎢⎣ −<sup>1</sup><sub>1 </sub>⎥⎤⎦, <em><u>m</u></em><sub>3 </sub>=⎡⎣⎢ <sup>−</sup><sub>2</sub><sup>2 </sup>⎤⎦⎥ <sub>  </sub>

⎣

<u>Σ</u>1=<u>Σ</u>2 =<u>Σ</u>3 =⎢⎡ ⎣   −11 −21 ⎤⎥ ⎦

<ul>

 <li>Give expressions for the discriminant functions <em>g</em><sub>1</sub>(<em><u>x</u></em>), <em>g</em><sub>2</sub>(<em><u>x</u></em>) and <em>g</em><sub>3</sub>(<em><u>x</u></em>) in terms of the given numbers, in simplest forms. <strong>Hint:</strong> before plugging in numbers, you can simplify the <em>g<sub>i </sub></em>(<em><u>x</u></em>) by dropping some terms.  Is the classifier linear, quadratic, or neither?</li>

 <li>Let . Give equations for the 3 decision boundaries, in simplest form.</li>

 <li>In (non-augmented) feature space, plot the class means, the 3 curves for <em>d<sub>M</sub></em><sup>2</sup>(<em><u>x</u></em>,<em><u>m</u><sub>i </sub></em>)=1, and the decision boundaries. Show clearly the decision regions and final boundaries.</li>

</ul>




<ol start="2">

 <li>A <em>Naïve Bayes</em> classifier is a Bayes classifier in which the features, conditioned on class, are assumed independent; thus:</li>

</ol>

<em>D p</em>(<em><u>x</u></em><em>S<sub>i</sub></em>)=∏ <em>p</em>(<em>x<sub>j </sub>S<sub>i</sub></em>) ∀<em>i </em>=1,!,<em>C </em>.

<em>          </em><em>j</em>=1

Most of the below is similar to your work for Problem 1.

For a Naïve Bayes (minimum error) classifier, let the given class-conditional densities and priors be:

<em>p</em>(<em>x S<sub>i </sub></em>)= <em>N</em>(<em>x</em>,<em><u>m</u><sub>i</sub></em>,<u><sup>Σ</sup></u><em><sub>i </sub></em>),   <em>i </em>=1, 2, 3

⎡ (σ<sub>1</sub>(<em>i</em>))2             0          ⎤ ⎥

⎢

<u>Σ</u><em>i </em>=⎢⎢⎢⎣              0         (σ2(<em>i</em>))2 ⎥⎥⎥ ⎦

<em>P</em>(<em>S</em><sub>1</sub>)=π<sub>1</sub>, <em>P</em>(<em>S</em><sub>2</sub>)=π<sub>2</sub>, <em>P</em>(<em>S</em><sub>3</sub>)=π<sub>3</sub>

<ul>

 <li>Write an expression for the discriminant functions <em>g<sub>i </sub></em>(<em><u>x</u></em>) , in the form:</li>

</ul>

<em>g</em><em>i </em>(<em><u>x</u></em>)=<em>w</em>1(1<em>i</em>)<em>x</em>12 +<em>w</em>1(2<em>i</em>)<em>x</em>1<em>x</em>2 +<em>w</em>2(<em>i</em>2)<em>x</em>22 +<em>w</em>1(<em>i</em>)<em>x</em>1+<em>w</em>2(<em>i</em>)<em>x</em>2 +<em>w</em>0(<em>i</em>)

and give expressions for all the weights in terms of given scalar quantities, in simplest (<em><sup>i</sup></em><sup>) </sup><em>m</em><sub>2</sub>(<em><sup>i</sup></em>)<sup>⎤</sup>⎥⎦<em>T   </em>.   form.  Let the mean vector of class <em>S<sub>i</sub></em>  be denoted <em><u>m</u><sub>i </sub></em>=<sup>⎡</sup>⎢⎣<em>m</em><sub>1</sub>

<ul>

 <li>Is the classifier quadratic, linear, or neither?</li>

 <li>For this part you are also given:</li>

</ul>

<em><u>m</u></em><sub>1</sub>=⎢⎣ ⎡   <sup>1</sup><sub>2 </sub>⎤⎥⎦ ,   <em><u>m</u></em><sub>2 </sub>=⎡⎢⎣ −<sup>1</sup><sub>1 </sub>⎤⎥⎦, <em><u>m</u></em><sub>3 </sub>=⎢⎣⎡ <sup>−</sup><sub>2</sub><sup>2 </sup>⎥⎦⎤ σ1(<em>i</em>))2 =σ12 =1, (σ2(<em>i</em>))2 =σ22 = 2, ∀<em>i</em>

<ul>

 <li>Give expressions for the discriminant functions <em>g</em><sub>1</sub>(<em><u>x</u></em>), <em>g</em><sub>2</sub>(<em><u>x</u></em>) and <em>g</em><sub>3</sub>(<em><u>x</u></em>) in terms of the given numbers, in simplest forms. <strong>Hint:</strong> before plugging in numbers, you can simplify the <em>g<sub>i </sub></em>(<em><u>x</u></em>) by dropping some terms.  Is the classifier linear, quadratic, or neither?</li>

 <li>Let . Give equations for the 3 decision boundaries, in simplest form.</li>

 <li>In (non-augmented) feature space, plot the class means, the 3 curves for <em>d<sub>M</sub></em><sup>2</sup>(<em><u>x</u></em>,<em><u>m</u><sub>i </sub></em>)=1, <em>i </em>=1,2,3, and the decision boundaries. Show clearly the decision regions and final boundaries.   <em>Problem 2 continues on next page… </em></li>

</ul>

<ul>

 <li>Compare your plot of 2(c)(iii) with your plot of 1(c)(iii). Does the dependence vs.</li>

</ul>

independence of features make a substantial difference in the decision boundaries and regions?




<ol start="3">

 <li>This problem uses the minimum risk criterion (instead of minimum error criterion) for classification (introduced in Lecture 21, covered in Discussion 12 and DHS 2.2). In this problem, please use our notation (<em> S<sub>i</sub></em> instead of <em><sub> </sub></em>ω<em><sub>i</sub></em> for class <em>i</em> ).</li>

</ol>

This problem is based on our 2-class tumor classification example.  Suppose the classconditional densities are known (or assumed) to be Gaussian:

<em>p</em>(<em>x S<sub>i </sub></em>)= <em>N</em>(<em><u>x</u></em>,<em><u>m</u><sub>i</sub></em>,<u><sup>Σ</sup></u><em><sub>i </sub></em>),   <em>i </em>=1, 2

For a Bayes minimum risk classifier, answer the parts below.

<ul>

 <li>Write the decision rule for a 2-class Bayes minimum risk classifier, in terms of conditional risks <em>R</em>(α<sub>1 </sub><em><u>x</u></em>) and <em>R</em>(α<sub>2 </sub><em><u>x</u></em>).  Then, write the decision rule in terms of <em>d</em><em>M</em>2(<em><u>x</u></em>,<em><u>m</u></em><em>i </em>), <u>Σ</u>1, <u>Σ</u>2 , λ11,λ12,λ21,λ22 , <em>P</em>(<em>S</em>1), and <em>P</em>(<em>S</em>2).</li>

</ul>

For parts (b)-(d) below, suppose also that on average, 80% of the tumors that are to be classified (based on their MRI images) are benign (class <em>S</em><sub>1</sub>), and the other 20% are cancerous (class <em>S</em><sub>2</sub>).

<ul>

 <li>Give estimates of the class priors <em>P</em>(<em>S</em><sub>1</sub>) and <em>P</em>(<em>S</em><sub>2</sub>).</li>

</ul>

For parts (c)-(e) below, suppose also that misclassifying a cancerous tumor as benign, is considered much worse than misclassifying a benign tumor as cancerous.  Thus we will use for our cost coefficients:

⎡⎢ ⎢⎣ λλ1211 λλ1222 ⎦⎤ ⎥⎥=⎣⎡⎢ 01 100 ⎤⎥⎦

Also, you are given that the mean vectors and covariance matrices for each class are known (or estimated) as:

<em><u>m</u></em>1=⎢⎡ ⎣   14 ⎤⎥⎦ , <em><u>m</u></em>2 =⎡⎢⎣ 42 ⎤⎥ ⎦

<u>Σ</u><sub>1</sub>=<u>Σ</u><sub>2 </sub>=⎢⎡ ⎣   −0<sub>0</sub>.5<sub>.5 </sub>−0<sub>2</sub>.5 ⎤⎥ ⎦




<ul>

 <li>Solve for the decision boundary and regions; that is, give an expression (in simplest form, based on the given numbers) for the decision rule. <em>Problem 3 continues on next page… </em></li>

 <li>Plot in 2D feature space, the class means, the 2 curves for <em>d<sub>M</sub></em><sup>2</sup>(<em><u>x</u></em>,<em><u>m</u><sub>i </sub></em>)=1, <em>i </em>=1,2, the decision boundary, and show the decision regions (by a small arrow at the boundary pointing into Γ<sub>1</sub>, or by labelling Γ<sub>1 </sub>andΓ<sub>2</sub>).</li>

 <li>If the guidelines for ordering an MRI change, and it is estimated that the data points coming in will be, on average, 50% benign and 50% cancerous, repeat part (d) (or add it to your part (d) plot, clearly labeled as (e)). How have the boundary and regions changed?</li>

</ul>








