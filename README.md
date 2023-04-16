**Mathematical Model on Climate Change**

Asiya Anas, Ashwin Nair, Faheena Thesni, Farsana, Govindram Niware

1.  School of Mathematics, Indian Institute of Science Education and
    > Research, Thiruvananthapuram

2.  School of Data Science, Indian Institute of Science Education and
    > Research, Thiruvananthapuram

> \* E-mail of the corresponding authors:
> [[[asiyaanas20@iisertvm.ac.in]{.underline}](mailto:asiyaanas20@iisertvm.ac.in)
> [[ashwinnair20@iisertvm.ac.in]{.underline}](mailto:ashwinnair20@iisertvm.ac.in)]{.mark}
>
> [[[faheenathes20@iisertvm.ac.in]{.underline}](mailto:faheenathes20@iisertvm.ac.in)]{.mark}
> [[[farsana20@iisertvm.ac.in]{.underline}](mailto:farsana20@iisertvm.ac.in)
> [[govindram20@iisertvm.ac.in]{.underline}](mailto:govindram20@iisertvm.ac.in)]{.mark}

**Abstract**

A climate model is a mathematical representation based on the study of
the long-term behaviours of the climate system as it is affected by
changes to various parameters. A differential equation model was
developed and verified using the mean global temperature annually,
forest area, and the daily amounts of precipitation. We mostly use the
model used in \[1\] and check to see how it fits on real world data to
check the effectiveness of the model described. One of our main
contributions involve realising the effect of temperature on forest area
and modelling the differential equation model described in \[1\] with
our modifications. This research looks at the long-term behavior of
rainfall as it is affected by changes in forest area and global warming.
To best capture the effects of severe weather hazards such as drought ,
global temperature and forest cover are considered annually, while
rainfall is considered seasonally. A differential equation model was
developed and validated using the annual mean global temperature, forest
area, and daily rainfall amounts.

**1. Introduction**

Climate is an inevitable part of Earth's atmosphere. Climate change is
an irreversible consequence of the global warming phenomenon.

Climate change models are essential tools for understanding and
predicting the complex interactions between Earth\'s atmosphere, oceans,
land surface, and biosphere. These models are designed to study the
impacts of climate change on the environment, economy, and society.

In this model, we will explore the impact of climate change on forest
areas, rainfall patterns, and temperature trends. The model will use
historical data to establish a baseline and then project future
scenarios based on various climate change scenarios. This model will
provide valuable insights for policymakers and conservationists who are
working to protect our ecosystem.

**1.1 Statement of the Problem**

Changes in climate have the potential to impact the economy and society.
In the past few years, climate change and its impact on daily life have
been a hot topic. It has grabbed the worldwide attention of scientists
and leaders, obliging them to take action against climate change. This
model is intended to answer the following questions:

1.  Can we formulate a mathematical model that establishes the
    > relationship between global temperature, annual precipitation and
    > forest coverage?

2.  What is the impact of rising rainfall trends on declining forest
    > areas and global temperature?

3.  How does global temperature change with forest area?

4.  Is our model capable of predicting future climate changes?

**2. The model**

**2.1 Assumptions**:

In order to build the model, the following assumptions are made:

\(i\) Global temperature appears to be increasing exponentially.
However, the global temperature cannot

continue to rise indefinitely. It should be constrained at some
temperature.

\(ii\) Today\'s forest area has decreased exponentially in comparison to
the past. Because the forest area

cannot fall below zero and cannot exceed the maximum area of the studied
region, it is an example of

logistic decay.

\(iii\) The amount of rainfall appears to be seasonal and thus periodic.
To capture seasonal rainfall, a second

order differential equation with a periodic solution should be
considered.

\(iv\) The decrease in forest area is inversely proportional to the rise
in the temperature and it is important to

not overlook the effect of temperature on forest area

\(v\) Sources of change in a particular variable is considered to be
zero from the other two variables.

**2.2 Variables**

Temperature: T

Rainfall: R

Forest Area: F

Time: t

**2.3 Constants**

1.  a~T~ : Rate of change of Temperature

2.  a~F~ : Rate of change of Forest area

3.  ⍺ : Rate of change of Rainfall

4.  b~T~ : Difference between two equilibrium points (T)

5.  b~f~ ; Difference between two equilibrium points (F)

6.  m~T~ : Minimum global temperature

7.  m~f~ : Minimum global Forest area

**2.4 General Model As Proposed in \[1\]:**

![](media/image1.png){width="3.0138265529308836in"
height="1.0083858267716534in"}

**2.5 Stability Analysis**

1\.

![](media/image7.png){width="3.125in" height="0.8645833333333334in"}

Therefore both critical solutions are stable

**2.**

> ![](media/image2.png){width="4.677083333333333in"
> height="0.8333333333333334in"}
>
> Therefore both equilibrium points are stable
>
> **3.**
>
> ![](media/image4.png){width="0.7916666666666666in" height="0.53125in"}
> ![](media/image6.png){width="0.8645833333333334in"
> height="0.6458333333333334in"}
>
> ![](media/image3.png){width="0.96875in" height="0.3854166666666667in"}
>
> (0,0) is a critical point (0,0) is the centre. Therefore, the solution
> is stable

**2.6 Results**

For testing of the model form \[1\] we have used the dataset \[4\] for
the global annual forest area data, \[2\] for the global temperature of
the earth and \[3\] for the seasonal rainfall data. We have the testing
the model above using python using the SciPy library, specifically we
have used the odeint() solver function in Scipy to solve the
differential equations discussed above

The forest area model results:

: ![](media/image8.png){width="3.621875546806649in"
height="2.5654943132108485in"}

The temperature model results:

![](media/image11.png){width="3.757292213473316in"
height="2.67911198600175in"}

The rainfall model results:

![](media/image10.png){width="3.877923228346457in"
height="2.6815419947506562in"}

**2.7 Modified General Model**

![](media/image5.png){width="3.2395833333333335in" height="1.0625in"}

**2.8 Variables**

1.  Temperature: T

2.  Rainfall: R

3.  Forest Area: F

4.  Time: t

**2.9 Constants**

1.  a~T~ : Rate of change of Temperature

2.  a~F~ : Rate of change of Forest area

3.  ⍺ : Rate of change of Rainfall

4.  b~T~ : Difference between two equilibrium points (T)

5.  b~f~ ; Difference between two equilibrium points (F)

6.  m~T~ : Minimum global temperature

7.  m~f~ : Minimum global Forest area

8.  c~f~ : Constant depicting the interaction between forest area and
    > temperature.

**2.10 Results for the Modified Model:**

For testing of the modified model we have used the dataset \[4\] for the
global annual forest area data, \[2\] for the global temperature of the
earth and \[3\] for the seasonal rainfall data. We are testing the model
above using python SciPy library, specifically we have used the odeint()
solver function in Scipy to solve the differential equations discussed
above

The forest area model results:

![](media/image9.png){width="3.6427088801399825in"
height="2.2557360017497814in"}

For better comparison with the original model from \[1\] and our new
model we also plotting the two of them together.

The comparison results are:

![](media/image12.png){width="3.7677088801399825in"
height="2.6010028433945758in"}

We can observe that for the most part our modified model is close to the
model defined by \[1\], but our model predictions are much better for
prediction for a long time as it is more general and takes the changing
temperature into account.

**3. Conclusion**

The relationship between global temperature dynamics, forest area, and
amounts of rainfall has been mathematically formulated. As mean
temperatures have risen, mean precipitation also has increased. This is
expected because evaporation increases with increasing temperature, and
there must be an increase in precipitation to balance the enhanced
evaporation

There is a decrease in forest area due to deforestation to inhabit the
increasing population.The modified model includes the interaction
between temperature and forest area taking into consideration of the
increasing risk of wild fire due to increase in temperature.

**References**

\[1\] Genet Mekonnen Assefa : Mathematical Model on the Effects of
Global Climate Change and Decreasing Forest Cover on Seasonal Rainfall
DOI: 10.7176/MTM/9-1-03

\[2\] Climate Change: Earth Surface Temperature Data:
https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data?resource=download

\[3\] Precipitation Dataset:
https://data.worldbank.org/indicator/AG.LND.PRCP.MM?end=2019&start=2019&view=bar

\[4\] Forest Area Dataset:

https://data.worldbank.org/indicator/AG.LND.FRST.K2?end=2020&start=1990&view=chart
