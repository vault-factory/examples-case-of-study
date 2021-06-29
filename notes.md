# Research notes

## terms
**vault:** a contract where can deposit token/cryptocurrency.
**yearn vault:** pool of funds with an associated strategy for maximising returns. (producing yield. yEarn = yield earn)
**vault strategy:** is a mix of differents actions that can be:
- supply collacteral to an token/cruptocurrencies
- borrowing other assets
- providing liquidity (a.k.a. LP)
- collecting trading fees
- farming other tokens and selling them for profit
- lending out coins
- liquidity mining (a.k.a. LM)

**Liquidity Provider:** someone who provide a pair of different tokens to a Liquidity Pool. (a.k.a. LP)

**Liquidity Pool:** are pools of tokens that are locked in a smart contract (at this part is same as a vault) and they are used to facilitate trading by providing liquidity (liquidity mining) and are extensively used by some of the decentralized exchanges a.k.a DEXes.

**Liquidity Tokens:** Whenever liquidity is deposited into a pool, unique tokens known as liquidity tokens are minted and sent to the provider’s address. These tokens represent a given liquidity provider’s contribution to a pool. The proportion of the pool’s liquidity provided determines the number of liquidity tokens the provider receives. If the provider is minting a new pool, the number of liquidity tokens they will receive will equal sqrt(x * y), where x and y represent the amount of each token provided.

**Liquidity Mining:** provide (stake) two coins (both as trading pairs) that they are used to facilitate trading  

**DEX:** Descentralized Exchanges

### about Yearn Vaults or yVaults:

yVaults has some rules:
- you receive the corresponding yTOKENS that can be redeemed for the underlying tokens
- you always withdraw the same asset that was initially deposited
- farmed tokens and accrued fees are sold for the main asset in the vault
- the amount that is withdrawn is the initial amount that was put in, plus the pool yield that was earned, minus the fees.


### commons useful variables

**in vaults:**
- deposits fees (a.k.a. entrance fee)
- management fee
- performance fee
- redemtion fee (a.k.a. exit fee)

**in strategies:**
- strategy holding (part that is invest)
- idle amount (part no invest, keep as liquid)
- gas fee (to subsidize the gas cost)
- strategy creator fee
- treasury thresold


NB: first we deploy the strategy then the vault that point to the strategy

