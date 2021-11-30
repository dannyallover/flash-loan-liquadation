# Flash Loan Liquadation
A smart contract that performs a flash loan based liquidation.
<br>
<br>
For the initial loan, a user borrowed USDT with WBTC as collateral. The loan becomes undercolatiralized as the price of WBTC falls; however, 
WBTC still remains more valuable than USDT, so we can make a profit by liquidating the loan. We do so by taking a flash loan: first, borrow USDT with ETH; 
second, pay back loan with USDT, third; convert the recieved collateral (WBTC) to WETH. This process results in a profit of ~43.81 ETH.

## Prerequisite
- You need to register an account on https://www.alchemy.com/ for access to an archive Ethereum node.

- You need to prepare the nodeJS environment for the project yourself, or have [docker](https://www.docker.com/) installed on your machine.
