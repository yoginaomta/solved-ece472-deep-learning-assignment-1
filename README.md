Download Link: https://assignmentchef.com/product/solved-ece472-deep-learning-assignment-1
<br>



<strong>          </strong>tldr: Perform linear regression of a noisy sinewave using a set of gaussian basis

<strong>         </strong>functions with learned location and scale parameters. Model parameters are

<strong><sup>           </sup></strong>learned with stochastic gradient descent. Use of automatic differentiation is

<strong>             </strong>required. Hint: note your limits

<strong>Problem Statement        </strong>Consider a set of scalars {<em>x</em><sub>1</sub><em>,x</em><sub>2</sub><em>,…,x<sub>N</sub></em>} drawn from U(0<em>,</em>1) <strong>012   </strong>and a corresponding set {<em>y</em><sub>1</sub><em>,y</em><sub>2</sub><em>,…,y<sub>N</sub></em>} where:




<table width="574">

 <tbody>

  <tr>

   <td width="46"> </td>

   <td width="496"><em>y<sub>i </sub></em>= sin(2<em>πx<sub>i</sub></em>)+ <em>ϵ<sub>i</sub></em>and <em>ϵ<sub>i </sub></em>is drawn from N(0<em>,σ</em><sub>noise</sub>). Given the following functional form:<em>y</em>ˆ<em><sub>i </sub></em>= ∑<em>w<sub>j</sub>ϕ<sub>j </sub></em>(<em>x<sub>i </sub></em>| <em>µ<sub>j</sub>,σ<sub>j</sub></em>)+ <em>b </em><em>M</em><em>j</em>=1with:</td>

   <td width="32">(1)(2)</td>

  </tr>

 </tbody>

</table>




(3)




<table width="501">

 <tbody>

  <tr>

   <td width="46">  </td>

   <td width="454">find estimates <sup>ˆ</sup><em>b</em>, {<em>µ</em>ˆ<em><sub>j</sub></em>}, {<em>σ</em>ˆ<em><sub>j</sub></em>}, and {<em>w</em>ˆ<em><sub>j</sub></em>} that minimize the loss function:</td>

  </tr>

 </tbody>

</table>

<strong><sup>4.   </sup></strong>for all (<em>x<sub>i</sub>,y<sub>i</sub></em>) pairs. Estimates for the parameters must be found using stochastic

<strong> </strong>gradient descent. A framework that supports automatic differentiation must be

<strong>  </strong>used. Set <em>N </em>= 50<em>,σ</em><sub>noise </sub>= 0<em>.</em>1. Select <em>M </em>as appropriate. Produce two plots. First,

<strong><sup> </sup></strong>show the data-points, a noiseless sinewave, and the manifold produced by the

regression model. Second, show each of the <em>M </em>basis functions. Plots must be of

<strong> </strong>suitable visual quality.<strong>   </strong>−4               −2                               0                                 2                                 4                                 −4                               −2                               0                                 2                                 4 x                              x

<strong><sup> </sup></strong>Figure 1: Example plots for models with equally spaced sigmoid and gaussian basis functions.


