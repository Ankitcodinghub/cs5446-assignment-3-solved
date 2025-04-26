# cs5446-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [CS5446 Assignment 3 Solved](https://www.ankitcodinghub.com/product/cs5446-assignment-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94835&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS5446 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

Problem 1: Q-Learning with Continuous State

Consider a system with a single continuous state variable x and actions a1 and a2. An agent can observe the value of the state variable as well as the reward in the observed state. Assume a discount factor γ = 0.9.

(a) AssumethatfunctionapproximationisusedwithQ(x,a1)=w0,1+w1,1x+w2,1×2 and Q(x, a2) = w0,2 + w1,2x + w2,2×2. Give the Q-learning update equations.

Q(x, a) ← Q(x, a) + α[R(x) + 0.9 max Q(x′, a′) − Q(x, a)], a′

where a′ ∈ a1, a2, α indicates learning rate and R is the reward.

(b) Assume that wi,j = 1 for all i, j. The following transition is observed: x = 0.5, observed reward r = 10, action a1, next state x = 1. What are the updated values of the parameters assuming a learning rate of 0.5?

wi,1 ←wi,1 +α[r+0.9 max Q(x′,a′)−Q(x,a1)]∂Q(x,a1),wherei=0,1,2; a′ ∈a1 ,a2 ∂ wi,1

wi,1 ← 1+0.5[10+0.9(1+1+1)−(1+0.5+0.25)]∂w0,1+0.5w1,1+0.25w2,1 , where i = 0, 1, 2; ∂ wi,1

w0,1 ← 1+5.475∗1 = 6.475;

w1,1 ← 1 + 5.475 ∗ 0.5 = 3.7375; w2,1 ← 1 + 5.475 ∗ 0.25 = 2.36875;

Problem 2: Policy Gradient with Continuous State

Assume that Q-function with function approximation is used together with the softmax function to form a policy πθ(s,a) = eQθ(s,a)/􏰀a′ eQθ(s,a′) . Assume that there are two actions with Q(x, a1) = w0,1 + w1,1x + w2,1×2 and Q(x, a2) = w0,2 + w1,2x + w2,2×2 for a real valued variable x.

<ol>
<li>(a) &nbsp;Give the update equations for the REINFORCE algorithm. Assume that the the return at the current step is G and the action taken is a1.wi,j ← wi,j + α ∗ G∇wi,j ln πwi,j (x, a1),

where i = 0, 1, 2, j = 1, 2, and α indicates learning rate.</li>
<li>(b) &nbsp;Assume that wi,j = 1 for all i, j and return G = 5 is received. What are the updated values of the parameters assuming x = 0.5 and a learning rate of 0.5?wi,j ←wi,j +α∗G∇wi,j lnπwi,j(x,a1),wherei=0,1,2andj=1,2;</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
w w

</div>
<div class="column">
0,1 1,1

</div>
<div class="column">
← 1 + 0.5 ∗ 5∇ ln w0,1

</div>
<div class="column">
ew0,1+0.5+0.25

ew0,1 +0.5+0.25 +e1+0.5+0.25

</div>
<div class="column">
= 1 + 2.5 ∗

</div>
<div class="column">
e = 1 + 1.25 = 2.25 e+e

</div>
</div>
<div class="layoutArea">
<div class="column">
← 1+0.5∗5∇

</div>
<div class="column">
w1,1

</div>
<div class="column">
ln

</div>
<div class="column">
e1+0.5w1,1+0.25 e1+0.5w1,1 +0.25 +e1+0.5+0.25

</div>
<div class="column">
= 1+2.5∗

</div>
<div class="column">
0.5e0.5 = 1+0.625 = 1.625 e0.5 +e0.5

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
CS 5446:

</div>
<div class="column">
AI Planning and Decision Making

</div>
</div>
<div class="layoutArea">
<div class="column">
w

w

w

</div>
<div class="column">
2,1 0,2

</div>
<div class="column">
= 1 + 2.5 ∗

=1+2.5∗ −e =1−1.25=0.25

</div>
</div>
<div class="layoutArea">
<div class="column">
← 1 + 0.5 ∗ 5∇ ln w2,1

←1+0.5∗5∇ ln w0,2

</div>
<div class="column">
e1+0.5+0.25w2,1 e1+0.5+0.25w2,1 +e1+0.5+0.25

e1+0.5+0.25 e1+0.5+0.25 +ew0,2 +0.5+0.25

</div>
<div class="column">
0.25e0.25 = 1.3125 e0.25 +e0.25

</div>
</div>
<div class="layoutArea">
<div class="column">
1,2 2,2

</div>
<div class="column">
← 1+0.5∗5∇ w1,2

</div>
<div class="column">
ln

</div>
<div class="column">
e1+0.5+0.25 e1+0.5+0.25 +e1+0.5w1,2 +0.25

</div>
<div class="column">
e+e

= 1+2.5∗ −0.5e0.5 = 1−0.625 = 0.325

</div>
</div>
<div class="layoutArea">
<div class="column">
w ← 1 + 0.5 ∗ 5∇

</div>
<div class="column">
w2,2

</div>
<div class="column">
ln e1+0.5+0.25 e1+0.5+0.25 +e1+0.5+0.25w2,2

</div>
<div class="column">
= 1 + 2.5 ∗ −0.25e0.25 = 0.6875 e0.25 +e0.25

</div>
</div>
<div class="layoutArea">
<div class="column">
e0.5 +e0.5

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
