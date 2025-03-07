# Using Yearn

Thanks to a feature called 'zap', it's extremely easy to deposit into any vault with almost any token.

Here's how it works:

First, **Connect your wallet** using the button at the top right corner. Multiple types of wallets are supported, but most people use [MetaMask](https://metamask.io/), which can be downloaded for free as a Chrome extension or through the Apple and Android app stores. Make sure that your wallet is connected to the Ethereum network.

<p align="center">
  <img width="900" height="305" src="https://i.imgur.com/XolXLi4.png" className="topRightImg"/>
</p>

## Yearn is multi-chain

Our products are currently on Ethereum and Fantom, with more to come.

Click on this button to select the network you would like to interact with:

![](https://i.imgur.com/cDKJDcx.png)

## If you **already have the required token** for the vault that you would like to deposit in:

1. Select the vault that you would like to deposit into.
2. Enter the amount of tokens you want to deposit into the vault. If you are depositing ETH, make sure you have enough ETH left over to pay for future transactions that you might need to make.

<p align="center">
  <img width="900" height="460" src="https://i.imgur.com/EmOAKlt.png" className="topRightImg"/>
</p>

3. Click 'Approve' or 'Deposit' button, depending on if you have previously approved
4. Your wallet will ask you to confirm the transaction. This will take about 3 minutes, but you can speed it up by [paying a higher gas fee to the network](https://blog.leverj.io/how-to-set-the-gas-limit-and-gas-price-in-metamask-1b33c38c32fd). If your transaction gets stuck, see [this guide](https://metamask.zendesk.com/hc/en-us/articles/360015489251-How-to-Speed-Up-or-Cancel-a-Pending-Transaction) on speeding up or cancelling the transaction.

<p align="center">
  <img width="258.75" height=" 459.75" src="https://i.imgur.com/qjryeGD.png" className="topRightImg"/>
</p>

6. When your transaction succeeds, you will see your deposited balance in the vault's interface, which should appear at the top of the vault list.

<p align="center">
  <img width="900" src="https://i.imgur.com/ICFADLL.jpeg"/>
</p>

When you're ready to withdraw:

1. Select the vault that you would like to withdraw from. Click the "Withdraw" tab

<p align="center">
  <img width="900" height="300" src="https://i.imgur.com/9Uw4oSB.png" className="topRightImg"/>
</p>

2. Enter the amount you want to withdraw, or click 'Max' to withdraw the entire balance.
3. Click 'Withdraw'
4. Your wallet will ask you to confirm the transaction. See step 4 above for more details.
5. When your transaction succeeds, the tokens will show up in your wallet again

## If you **don't have the required token** for the vault that you would like to deposit in:

This can be a common occurrence, because many of Yearn's vaults generate yield by using [Curve Finance](https://curve.finance/) liquidity provider (LP) tokens, which are acquired through depositing into a Curve pool.

So for instance, if you would rather deposit into the ibJPY vault instead of the ETH vault, and accept the additional risk that comes with the curve pool and an ETH derivative (stETH) in return for higher yield, but you only have ETH in your wallet, your ETH will need to be converted to a ibJPY token before it is accepted in the vault.

Thankfully, due to Yearn's 'zap' feature, this can all be done in the same transaction as your deposit. Here's how it works using the ibJPY vault as an example:

**NOTE:** Zapping a token into a vault will require more transactions than depositing the native token. This means you will be paying more in gas and potentially lose value to slippage when the token is swapped or deposited into a pool. Yearn limits slippage to 1% and the transaction will fail if slippage exceeds that, in which case you will have to swap or deposit the tokens manually. See our [zap](https://docs.yearn.finance/yearn-finance/yvaults/overview#zap-in-with-any-asset) section for more details.

1. Select the ibJPY vault
2. Click the dropdown box by the 'Approve' or 'Deposit' button
3. Select which token you would like to be converted into ibJPY. It will only display the tokens that are in your wallet.

<p align="center">
  <img width="900" src="https://i.imgur.com/IbYRzDN.png"/>
</p>

4. Enter the amount of tokens you would like to deposit and click 'Approve' or 'Deposit' depending on whether or not you have previously approved the token.
5. Confirm the transaction through your wallet. See step 4 in the section above for more details.
6. When your transaction succeeds, you will see your deposited balance in the vault's interface, which should appear at the top of the vault list.

When you're ready to withdraw:

1. Select the ibJPY vault
2. Click the dropdown box by the 'Withdraw' button

<p align="center">
  <img width="900" src="https://i.imgur.com/t0VEznT.png"/>
</p>

3. Select which asset you would like to receive upon withdrawal. Your options will be the ibJPY, ETH, BTC, DAI, USDC or USDT
4. Enter the amount you want to withdraw, or click 'Max' to withdraw the entire balance.
5. Confirm the approval if needed, and then approve the withdrawal transaction.
6. When your transaction succeeds, the tokens will show up in your wallet again

## Customization

Personalize your Yearn experience with customizations, in [Settings](https://yearn.finance/#/settings).
<p align="center">
  <img width="900" src="https://i.imgur.com/Ujduvty.png"/>
</p>

### Slippage Tolerance
Change your slippage preferences to one of three preset options listed. Learn more about slippage [here](/resources/defi-glossary#slippage)
### Themes
View Yearn.Finance with community-created themes or [create a custom theme](https://github.com/yearn/yearn-finance-v3/tree/develop/src/client/themes) to suit your style.

## Tools to track your funds

If you would like to see how your USD balance changes while your assets are in a vault, connect your wallet to [zapper.fi](https://zapper.fi) or a similar portfolio tracking product. This is also the easiest way to tell how much profit the vault has made for you.

Your balance WILL NOT increase continuously. Profit will be distributed to your share of the vault when the harvest() function is called, which happens on a fluctuating basis.

Community resources to monitor your returns:

- [Zapper](https://zapper.fi/)
- [Zerion](https://app.zerion.io/)
- [yVault ROI](https://yvault-roi.netlify.app/)
- [Trackavault](https://trackavault.com/)
