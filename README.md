# Interest Rate Futures and Valuation



Interest Rate Future Definition
An interest rate future is a futures contract between the buyer and seller to deliver an interest bearing asset, that allows the buyer and seller to lock in the price of the interest bearing asset for a future date. The most popular interest rate future is Eurodollar future.
Eurodollar futures contract is a cash-settled futures contract. The underlying instrument in Eurodollar futures is a Eurodollar time deposit having a principal value of $1,000,000 with a three-month maturity. Eurodollar futures prices are expressed numerically using 100 minus the implied 3-month U.S. dollar LIBOR interest rate. In this way, a Eurodollar future price of $98 reflects an implied settlement interest rate of 2%.
	Interest rate futures are used to hedge against interest rate risk. Investors can use Eurodollar futures to secure an interest rate for money it plans to borrow or lend in the future. Interest rate futures are mainly listed for 3-month Eurodollar, 1-month LIBOR, 1-month banker’s acceptance futures and 3-month banker’s acceptance futures.
Advantages of trading interest rate futures
Interest rate futures are used to hedge against interest rate risk. Investors can use interest rate futures to secure an interest rate for money it plans to borrow or lend in the future.  Futures markets tend to be more liquid than underlying cash markets.
Other benefits
	Price transparency and liquidity
	Immediate execution and confirmation
	Reduction of counterparty risk
	Centralized clearing.

Valuation
The price of an interest rate future is quoted by the exchange. A model is mainly used for calculating sensitivities and managing market risk.

The present value of an interest rate future is given by
PV(t)=n(F_T-F_0 )
where
	F_T=100-y(t:T,T_u) – future contract price at the valuation date
	t – valuation date
	T – maturity date of the future contract
	T_u – maturity date of the underlying rate, usually T_u=T+3month
	y(t:T,T_u ) – annually compounded forward yield for forward period (T, T_u)
	n – contract size
	F_o – quoted future contract price at the trade date T_0, T_0≤t≤T

Practical Notes
	You need to construct an interest zero rate curve by bootstring some most liquity interest rate instruments. FinPricing provides useful tools to build various curves, such as interest rate base curve, basis curve, OIS curve, bond curve, treasury curve, etc. <a href="/curveVolList.html">Go to the list of the tools</a>
	The forward yield is derived from the interest rate zero curve by calculating the annually compounded forward rate between the maturity date of the futures contract and the maturity date of the underlying rate.
	Theoretically a convexity adjustment is needed for pricing a future contract. However, the impact is small.

A Real World Example
Interest rate future specification
Buy Sell	Buy
Currency	USD
Contract Size	10000
First Delivery Date	5/30/2018
Last Delivery Date	6/29/2018
Future Maturity Date	6/18/2018
Tenor	3M
Future Ticker	EDM18
Future Ticker Size	100
Future Ticker Value	25
Number of Contract	100
Quote Price	98.405
Trade Date	12/2/2016


Reference:

https://finpricing.com/lib/EqConvertible.html

https://github.com/alanwhite1203/irFuture/raw/main/IrFuture-34.pdf

