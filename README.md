# Compound Option Valuation

A vanilla compound option is defined as a European vanilla option upon another European vanilla option,
which may be called underlying vanilla option. There are four types of compound options: call-on-call,
call-on-put, put-on-call and put-on-put. Due to the call-put parity, basically, we only need to consider call-on-call and call-on-put. In this report, under the assumption that the asset price, which is the underlyer of the underlying option, follows geometrical Brownian motion and that risk-free short rate, dividend yield and volatility are deterministic, we present Black-Scholes/Merton’s analytical close form pricing formula for vanilla compound options.

Let {St} be the price of a given asset which follows the following SDE

 

where {Wt} is a standard R-valued Wiener process, ¹t and ¾t are deterministic drift term and volatility,
respectively. Let rt be the deterministic risk-free short interest rate. For t < s, let us define

 

The discounting factor from s back to t, denoted by df(t; s), can be written as

 

and a forward price seen at t matured at s, denoted by F(t; s), can be written as

 

Let t < T and ST = eZT . Then we have

 

Further, Let t < T1 < T2, ST1 = eZ1 and ST2 = eZ2 . Then, Z1 »t N(m1; v1), Z2 »t N(m2; v2), and relative to the time of t, (Z1;Z2) is jointly normal distributed with the following correlation coefficient

 

Let f(¢; ¢) be the joint density function of (Z1;Z2) relative to time t, f1( ¢ ) is the density function of Z1
relative to time t and f2j1( ¢ ; ¢ ) is the density function of Z2 conditional on Z1 relative to time t. Clearly,
we have

 

where

 

Let T be a maturity of the compound option with a strike K > 0, T1 > T be the maturity of the underlying
option with a strike K1 > 0 and a call-put index °1. Then the compound option payoff at the maturity of
T becomes

 

We have

 

After substituting

 
In the following section, we will obtain analytical close form pricing formulae for the call-on-call and
call-on-put compound options.

The price dynamic follows:
 

References:

https://finpricing.com/FinPricing-ProductBrochure.pdf
