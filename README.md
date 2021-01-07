# Bitbns Python API

This project is designed to assist you make your own projects that interact with the Bitbns API.  This project seeks to have complete API coverage excluding WebSockets which would be released in the future version.

<code><b>Use Python 3.7+</b></code><br><br>

<h3>Installation</h3>
<code> sudo -H pip3 install python-socketio </code>
<br>
<code> pip3 install bitbnspy </code>

<h3> Getting Started </h3>

```
from bitbnspy import bitbns
key = 'yourKey'
secretKey = 'yourSecreatKey'
bitbnsObj = bitbns(key, secretKey)
print(bitbnsObj.getSellOrderBook('XRPUSDT'))
```

<br>

<h2>API Access</h2>
<div id ="api_summary_table" style ="border:1px solid">
  <table style = "width:55%">
    <tr>
      <th>PERMISSIONS</th>
      <th>Read</th>
      <th>Write</th>
    </tr>
    <tr>
      <th></th>
      <th></th>
      <th></th>
    </tr>
    <tr>
      <th>List Open Orders</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>List Open Stop Limit</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Api Usages Status</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Current Coin Balance</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Deposit History</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Withdrawal History</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Order Status</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
    <tr>
      <th>Buy Stop Loss Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Sell Stop Loss Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Buy Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Sell Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Get Coin Address</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
     <tr>
      <th>Cancel Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Cancel Stop Loss Order</th>
      <th>&#x2716;</th>
      <th>&#10003;</th>
    </tr>
     <tr>
      <th>Platform Status</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
     <tr>
      <th>Ticker API</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
      <tr>
      <th>Buy OrderBook</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
      <tr>
      <th>Sell OrderBook</th>
      <th>&#10003;</th>
      <th>&#x2716;</th>
    </tr>
  </table>
</div>

<h2>Minimum Volume allowed of supporting currencies</h2>
<table>
    <tr>
      <th>COIN NAME</th>
      <th>SYMBOL</th>
      <th>MINIMUM VOLUME ALLOWED</th>
      <th>MAXIMUM VOLUME ALLOWED</th>
    </tr>
    <tr>
      <th>Bitcoin</th>
      <th>BTC</th>
      <th>0.001</th>
      <th>20</th>
    </tr>
    <tr>
      <th>Ripple</th>
      <th>XRP</th>
      <th>50</th>
      <th>500000</th>
    </tr>
    <tr>
      <th>Neo</th>
      <th>NEO</th>
      <th>4</th>
      <th>10000</th>
    </tr>
    <tr>
      <th>Gas</th>
      <th>GAS</th>
      <th>13</th>
      <th>10000</th>
    </tr>
    <tr>
      <th>Stellar</th>
      <th>XLM</th>
      <th>300</th>
      <th>500000</th>
    </tr>
    <tr>
      <th>Ethereum</th>
      <th>ETH</th>
      <th>0.32</th>
      <th>20</th>
    </tr>
    <tr>
      <th>Bitcoin Cash</th>
      <th>BCH</th>
      <th>0.15</th>
      <th>200</th>
    </tr>
    <tr>
      <th>Tron</th>
      <th>TRX</th>
      <th>2800</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Cardano</th>
      <th>ADA</th>
      <th>880</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>VeChain</th>
      <th>VET</th>
      <th>5800</th>
      <th>20000</th>
    </tr>
    <tr>
      <th>Verge</th>
      <th>XVG</th>
      <th>4550</th>
      <th>2000000</th>
    </tr>
     <tr>
      <th>Dash</th>
      <th>DASH</th>
      <th>0.42</th>
      <th>200</th>
    </tr>
     <tr>
      <th>DigixDAO</th>
      <th>DGD</th>
      <th>1.5</th>
      <th>200</th>
    </tr>
     <tr>
      <th>LiteCoin</th>
      <th>LTC</th>
      <th>1.2</th>
      <th>150</th>
    </tr>
     <tr>
      <th>Augur</th>
      <th>REP</th>
      <th>6</th>
      <th>500</th>
    </tr>
    <tr>
      <th>Qtum</th>
      <th>QTUM</th>
      <th>17</th>
      <th>1000</th>
    </tr>
    <tr>
      <th>Lisk</th>
      <th>LSK</th>
      <th>24</th>
      <th>1000</th>
    </tr>
    <tr>
      <th>OmiseGo</th>
      <th>OMG</th>
      <th>21</th>
      <th>1000</th>
    </tr>
    <tr>
      <th>Waves</th>
      <th>WAVES</th>
      <th>34</th>
      <th>1000</th>
    </tr>
    <tr>
      <th>Ontology</th>
      <th>ONT</th>
      <th>35</th>
      <th>1000</th>
    </tr>
    <tr>
      <th>0x</th>
      <th>ZRX</th>
      <th>10</th>
      <th>3000</th>
    </tr>
    <tr>
      <th>Power Ledger</th>
      <th>POWR</th>
      <th>400</th>
      <th>8000</th>
    </tr>
    <tr>
      <th>PolyMath</th>
      <th>POLY</th>
      <th>324</th>
      <th>10000</th>
    </tr>
    <tr>
      <th>Tether</th>
      <th>USDT</th>
      <th>5</th>
      <th>5000</th>
    </tr>
    <tr>
      <th>Sia</th>
      <th>SC</th>
      <th>10000</th>
      <th>1000000</th>
    </tr>
    <tr>
      <th>NEM</th>
      <th>XEM</th>
      <th>564</th>
      <th>5000000</th>
    </tr>
    <tr>
      <th>DeepBrain Chain</th>
      <th>DBC</th>
      <th>9400</th>
      <th>500000</th>
    </tr>
    <tr>
      <th>MONERO</th>
      <th>XMR</th>
      <th>0.7</th>
      <th>200</th>
    </tr>
    <tr>
      <th>DogeCoin</th>
      <th>DOGE</th>
      <th>18000</th>
      <th>1000000</th>
    </tr>
    <tr>
      <th>Electroneum</th>
      <th>ETN</th>
      <th>4000</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>EOS</th>
      <th>EOS</th>
      <th>15</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Zilica</th>
      <th>ZIL</th>
      <th>2000</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Digibyte</th>
      <th>DGB</th>
      <th>3000</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>ICON</th>
      <th>ICX</th>
      <th>105</th>
      <th>20000</th>
    </tr>
    <tr>
      <th>Request</th>
      <th>REQ</th>
      <th>1500</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>QLC Chain</th>
      <th>QLC</th>
      <th>1500</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>Wan Chain</th>
      <th>WAN</th>
      <th>70</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>Achain</th>
      <th>ACT</th>
      <th>2500</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>Bluzelle</th>
      <th>BLZ</th>
      <th>500</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Substratum</th>
      <th>SUB</th>
      <th>600</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Loopring</th>
      <th>LRC</th>
      <th>600</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Nexo</th>
      <th>NEXO</th>
      <th>450</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Effect.Ai</th>
      <th>EFX</th>
      <th>5000</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Apex</th>
      <th>CPX</th>
      <th>2500</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>LOOM Network</th>
      <th>LOOM</th>
      <th>500</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>eosDAC</th>
      <th>EOSDAC</th>
      <th>1600</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Storm</th>
      <th>STORM</th>
      <th>8000</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Golem</th>
      <th>GNT</th>
      <th>400</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>PundiX</th>
      <th>NPXS</th>
      <th>40000</th>
      <th>2000000</th>
    </tr>
    <tr>
      <th>Ethereum Classic</th>
      <th>ETC</th>
      <th>10</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>DENT</th>
      <th>DENT</th>
      <th>30</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>CloakCoin</th>
      <th>CLOAK</th>
      <th>25</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Komodo</th>
      <th>KMD</th>
      <th>55</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>GroestlCoin</th>
      <th>GRS</th>
      <th>150</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>LinkEye</th>
      <th>LET</th>
      <th>10000</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>Phantasma</th>
      <th>SOUL</th>
      <th>600</th>
      <th>200000</th>
    </tr>
    <tr>
      <th>BNS token</th>
      <th>BNS</th>
      <th>300</th>
      <th>200000</th>
    </tr>
</table>


<h3>Getting Started</h3><br>
<pre>
from bitbns import bitbnsApi
apiKey = 'API-KEY'
apiSecretKey = 'API-SECRET-KEY'

bitbnsObj = bitbnsApi(apiKey, apiSecretKey)
</pre>


<b>Getting Platform Status</b>
<pre>
bitbnsObj.platformStatus();
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  data: {
    BTC: {
      status: 1
    },
    ETH: {
      status: 1
    },
    XRP: {
      status: 1
    }
  },
  status: 1,
  error: null
}

Explanation of fields:
status -> whether the coin is live on platform
   </pre>
</details>
<b>Getting latest price of a symbol</b>
Inputting Invalid crypto name would return "undefined" as the price.
<pre>
bitbnsObj.getTickerApi('BTC')
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": {
    "BTC": {
      "highest_buy_bid": 484159.43,
      "lowest_sell_bid": 494800,
      "last_traded_price": 494805.29
    }
  },
  "status": 1,
  "error": null
}

Explanation of fields:
highest_buy_bid -> top entry of buy order book
lowest_sell_bid -> top entry of sell order book
last_traded_price -> price at which the last trade had happened
   </pre>
</details>

<b>Getting latest price of few symbols</b>
<pre>
bitbnsObj.getTickerApi('BTC,ETH')
</pre>
<details>
 <summary>
    View Response
 </summary>
 <pre>
    {
  "data": {
    "BTC": {
      "highest_buy_bid": 484159.43,
      "lowest_sell_bid": 494800,
      "last_traded_price": 494805.29
    },
    "ETH": {
      "highest_buy_bid": 13205.01,
      "lowest_sell_bid": 13440,
      "last_traded_price": 13450
    }
  },
  "status": 1,
  "error": null
}

Explanation of fields:
highest_buy_bid -> top entry of buy order book
lowest_sell_bid -> top entry of sell order book
last_traded_price -> price at which the last trade had happened
 </pre>
</details>

<b>Getting latest price of all symbols</b>
<pre>
bitbnsObj.getTickerApi('')
</pre>

<details>
  <summary>
   View Response
  </summary>
<pre>
  {
  "data": {
    "BTC": {
      "highest_buy_bid": 480059.8,
      "lowest_sell_bid": 489000,
      "last_traded_price": 480059.8
    },
    "XRP": {
      "highest_buy_bid": 20,
      "lowest_sell_bid": 20.16,
      "last_traded_price": 20.16
    },
    "NEO": {
      "highest_buy_bid": 1301,
      "lowest_sell_bid": 1349.99,
      "last_traded_price": 1331.92
    },
    "GAS": {
      "highest_buy_bid": 406.96,
      "lowest_sell_bid": 418.46,
      "last_traded_price": 418.46
    },
    "ETH": {
      "highest_buy_bid": 13350,
      "lowest_sell_bid": 13660.5,
      "last_traded_price": 13350
    },
    "XLM": {
      "highest_buy_bid": 14.75,
      "lowest_sell_bid": 14.77,
      "last_traded_price": 14.77
    },
    "RPX": {
      "highest_buy_bid": 0.77,
      "lowest_sell_bid": 0.82,
      "last_traded_price": 0.8
    },
    "DBC": {
      "highest_buy_bid": 0.73,
      "lowest_sell_bid": 0.77,
      "last_traded_price": 0.72
    },
    "LTC": {
      "highest_buy_bid": 3680,
      "lowest_sell_bid": 3800,
      "last_traded_price": 3800
    },
    "XMR": {
      "highest_buy_bid": 7555,
      "lowest_sell_bid": 8000,
      "last_traded_price": 7600
    },
    "DASH": {
      "highest_buy_bid": 13500,
      "lowest_sell_bid": 14500,
      "last_traded_price": 13500
    },
    "DOGE": {
      "highest_buy_bid": 0.47,
      "lowest_sell_bid": 0.49,
      "last_traded_price": 0.49
    },
    "BCH": {
      "highest_buy_bid": 33600,
      "lowest_sell_bid": 34997,
      "last_traded_price": 34998
    },
    "SC": {
      "highest_buy_bid": 0.38,
      "lowest_sell_bid": 0.42,
      "last_traded_price": 0.42
    },
    "TRX": {
      "highest_buy_bid": 1.35,
      "lowest_sell_bid": 1.36,
      "last_traded_price": 1.35
    },
    "ETN": {
      "highest_buy_bid": 0.38,
      "lowest_sell_bid": 0.39,
      "last_traded_price": 0.39
    },
    "ONT": {
      "highest_buy_bid": 126.01,
      "lowest_sell_bid": 136.1,
      "last_traded_price": 136.82
    },
    "ZIL": {
      "highest_buy_bid": 2.37,
      "lowest_sell_bid": 2.5,
      "last_traded_price": 2.51
    },
    "EOS": {
      "highest_buy_bid": 365.51,
      "lowest_sell_bid": 375.1,
      "last_traded_price": 385
    },
    "POLY": {
      "highest_buy_bid": 10.01,
      "lowest_sell_bid": 10.04,
      "last_traded_price": 10.04
    },
    "DGB": {
      "highest_buy_bid": 1.6,
      "lowest_sell_bid": 1.83,
      "last_traded_price": 1.82
    },
    "NCASH": {
      "highest_buy_bid": 0.35,
      "lowest_sell_bid": 0.36,
      "last_traded_price": 0.36
    },
    "ADA": {
      "highest_buy_bid": 4.97,
      "lowest_sell_bid": 5.09,
      "last_traded_price": 4.92
    },
    "ICX": {
      "highest_buy_bid": 40.01,
      "lowest_sell_bid": 45.5,
      "last_traded_price": 40.25
    },
    "VEN": {
      "highest_buy_bid": 0.96,
      "lowest_sell_bid": 1.15,
      "last_traded_price": 1.15
    },
    "OMG": {
      "highest_buy_bid": 239.72,
      "lowest_sell_bid": 267.71,
      "last_traded_price": 267.71
    },
    "REQ": {
      "highest_buy_bid": 2.22,
      "lowest_sell_bid": 2.39,
      "last_traded_price": 2.3
    },
    "DGD": {
      "highest_buy_bid": 2385,
      "lowest_sell_bid": 3000,
      "last_traded_price": 2385
    },
    "QLC": {
      "highest_buy_bid": 3.3,
      "lowest_sell_bid": 3.96,
      "last_traded_price": 3.4
    },
    "POWR": {
      "highest_buy_bid": 10.02,
      "lowest_sell_bid": 11.4,
      "last_traded_price": 10.01
    },
    "WPR": {
      "highest_buy_bid": 1.18,
      "lowest_sell_bid": 1.25,
      "last_traded_price": 1.17
    },
    "WAVES": {
      "highest_buy_bid": 150.1,
      "lowest_sell_bid": 179,
      "last_traded_price": 150
    },
    "WAN": {
      "highest_buy_bid": 58.51,
      "lowest_sell_bid": 69.9,
      "last_traded_price": 53.55
    },
    "ACT": {
      "highest_buy_bid": 2.21,
      "lowest_sell_bid": 2.68,
      "last_traded_price": 2.21
    },
    "XEM": {
      "highest_buy_bid": 5.7,
      "lowest_sell_bid": 7.51,
      "last_traded_price": 10
    },
    "XVG": {
      "highest_buy_bid": 0.89,
      "lowest_sell_bid": 0.92,
      "last_traded_price": 0.88
    },
    "BLZ": {
      "highest_buy_bid": 7.61,
      "lowest_sell_bid": 7.8,
      "last_traded_price": 7.8
    },
    "SUB": {
      "highest_buy_bid": 7.06,
      "lowest_sell_bid": 8.5,
      "last_traded_price": 7.45
    },
    "LRC": {
      "highest_buy_bid": 6.5,
      "lowest_sell_bid": 9.95,
      "last_traded_price": 6.7
    },
    "NEXO": {
      "highest_buy_bid": 3.91,
      "lowest_sell_bid": 4.19,
      "last_traded_price": 3.91
    },
    "EFX": {
      "highest_buy_bid": 0.69,
      "lowest_sell_bid": 0.9,
      "last_traded_price": 0.7
    },
    "CPX": {
      "highest_buy_bid": 1.05,
      "lowest_sell_bid": 1.27,
      "last_traded_price": 1.05
    },
    "ZRX": {
      "highest_buy_bid": 38.09,
      "lowest_sell_bid": 39.49,
      "last_traded_price": 37.77
    },
    "REP": {
      "highest_buy_bid": 1050,
      "lowest_sell_bid": 1200,
      "last_traded_price": 1025
    },
    "LOOM": {
      "highest_buy_bid": 5.06,
      "lowest_sell_bid": 6.7,
      "last_traded_price": 6.7
    },
    "EOSD": {
      "highest_buy_bid": 3.51,
      "lowest_sell_bid": 3.88,
      "last_traded_price": 3.51
    },
    "STORM": {
      "highest_buy_bid": 0.47,
      "lowest_sell_bid": 0.5,
      "last_traded_price": 0.48
    },
    "GNT": {
      "highest_buy_bid": 9.25,
      "lowest_sell_bid": 9.26,
      "last_traded_price": 9.26
    },
    "QTUM": {
      "highest_buy_bid": 235,
      "lowest_sell_bid": 288.97,
      "last_traded_price": 247.69
    },
    "QKC": {
      "highest_buy_bid": 1.86,
      "lowest_sell_bid": 2.34,
      "last_traded_price": 1.76
    },
    "LSK": {
      "highest_buy_bid": 230,
      "lowest_sell_bid": 286,
      "last_traded_price": 230
    },
    "NPXS": {
      "highest_buy_bid": 0.11,
      "lowest_sell_bid": 0.12,
      "last_traded_price": 0.11
    },
    "USDT": {
      "highest_buy_bid": 74.12,
      "lowest_sell_bid": 77,
      "last_traded_price": 74.11
    },
    "ETC": {
      "highest_buy_bid": 804.02,
      "lowest_sell_bid": 850,
      "last_traded_price": 804
    },
    "DENT": {
      "highest_buy_bid": 0.15,
      "lowest_sell_bid": 0.17,
      "last_traded_price": 0.17
    },
    "CLOAK": {
      "highest_buy_bid": 120.51,
      "lowest_sell_bid": 159.92,
      "last_traded_price": 135
    },
    "KMD": {
      "highest_buy_bid": 70,
      "lowest_sell_bid": 77,
      "last_traded_price": 77.6
    },
    "GRS": {
      "highest_buy_bid": 35,
      "lowest_sell_bid": 39.4,
      "last_traded_price": 38.4
    },
    "RAM": {
      "highest_buy_bid": 0.38,
      "lowest_sell_bid": 0.4,
      "last_traded_price": 0.38
    },
    "LET": {
      "highest_buy_bid": 0.64,
      "lowest_sell_bid": 0.68,
      "last_traded_price": 0.68
    },
    "SOUL": {
      "highest_buy_bid": 2.26,
      "lowest_sell_bid": 2.71,
      "last_traded_price": 2.7
    },
    "PHX": {
      "highest_buy_bid": 0.77,
      "lowest_sell_bid": 0.82,
      "last_traded_price": 0.8
    },
    "VET": {
      "highest_buy_bid": 0.96,
      "lowest_sell_bid": 1.15,
      "last_traded_price": 1.15
    },
    "TST": {
      "highest_buy_bid": 23,
      "lowest_sell_bid": 27.5,
      "last_traded_price": 25
    }
  },
  "status": 1,
  "error": null
}
</pre>
</details>

<b>Getting current balance of crypto asset</b><br>
Inputing "INR" in place of crypto asset would list your inr balance .
<pre>
bitbnsObj.currentCoinBalance('BTC')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": {
    "inorderBTC": 8.34,
    "availableorderBTC": 15.76
  },
  "status": 1,
  "error": null
}

Explanation of fields:
inorderBTC -> volume which is the order book
availableorderBTC -> volume which is present in wallet
  </pre>
</details>

<b>Get Deposit History</b><br>
<pre>
bitbnsObj.depositHistory('BTC', 0)
</pre>


<details>
  <summary>
   View Response
  </summary>
  <pre>
 {
  data: [
    {
      type: 'BTC deposited',
      typeI: 1,
      amount: 0.00159302,
      date: '2018-08-21T14:35:02.000Z',
      unit: 'BTC',
      factor: 100000000,
      fee: 0,
      delh_btc: 0,
      delh_inr: 0,
      rate: 0,
      del_btc: 159302,
      del_inr: 0
    },
    {
      type: 'BTC deposited',
      typeI: 1,
      amount: 0.00142951,
      date: '2018-08-21T14:35:02.000Z',
      unit: 'BTC',
      factor: 100000000,
      fee: 0,
      delh_btc: 0,
      delh_inr: 0,
      rate: 0,
      del_btc: 142951,
      del_inr: 0
    }
  ],
  status: 1,
  error: null
}

Explanation of fields:
type -> type of action
typeI -> action id
amount -> the amount deposited
date -> the time at which this event occured
unit -> the symbol name of coin
factor -> the division factor
del_btc -> delta changes in normal wallet of coin
del_inr -> delta changes in normal inr wallet
delh_btc -> delta changes in hold wallet of coin
  </pre>
</details>


<b>Get Withdrawal History</b><br>
<pre>bitbnsObj.withdrawHistory('XRP', 0)</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
{
  data: [
    {
      type: 0,
      amount: 1.1,
      unit: 'XRP',
      hash: '42DAD88011C178DCAA1587ABA4458F4D535B30248650A6C353E5E2527',
      fee: 0.1,
      to: 'rB1za2ZVgqvrNB7u8LbVN61k5n1ByBUtXCA',
      status: '-1',
      canSendMail: 0,
      cancelable: -1,
      refer: 5339918,
      expTime: 'XRP withdraw done'
    },
    {
      type: 0,
      amount: 100,
      unit: 'XRP',
      hash: '12520219872260A25457E4D03C8F82F696A23EEA558B693B90FF080C5',
      fee: 0.1,
      to: 'rLdBnLq5C13ood9wdjY9ZCdgycK8KGevkUj',
      status: '-1',
      canSendMail: 0,
      cancelable: -1,
      refer: 6531933,
      expTime: 'XRP withdraw done'
    }
  ],
  status: 1,
  error: null
}
  </pre>
</details>


<b>List Open Orders</b><br>
<pre>
bitbnsObj.listOpenOrders('BTC')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": [
    {
      "entry_id": 322,
      "btc": 48,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 323,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 324,
      "btc": 100,
      "r ate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 325,
      "btc": 100,
      "rate": 25,
      "time": "2018-0 9-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 326,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "t ype": 1,
      "status": 0
    },
    {
      "entry_id": 327,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "e ntry_id": 328,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 329,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 330,
      "btc": 100,
      "rate": 25,
      "time": "201 8-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 331,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 332,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 333,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 334,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:29:52.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 337,
      "btc": 100,
      "rate": 25,
      "time": " 2018-09-10T12:45:51.000Z",
      "type": 1,
      "status": 0
    },
    {
      "entry_id": 338,
      "btc": 100,
      "rate": 25,
      "time": "2018-09-10T12:46:01.00 0Z",
      "type": 1,
      "status": 0
    }
  ],
  "status": 1,
  "error": null
}

Explanation of fields:
entry_id -> the unique id assigned to the order
btc -> the volume of the coin
rate -> the rate at which the order was placed
time -> the timestamp at which the order was placed
type -> 1 for sell and 0 for buy order
status -> -1 for cancelled , 0 for not processed , 1 for partially executed, 2 for fully executed
  </pre>
</details>

<b>List Open Stop Loss Orders</b><br>
<pre>
bitbnsObj.listOpenStopOrders('TST')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  data: [
    {
      entry_id: 28816,
      btc: 40,
      rate: 25,
      t_rate: 24.5,
      type: 1,
      status: 0
    }
  ],
  status: 1,
  error: null
}

Explanation of fields:
entry_id -> the unique id assigned to the order
btc -> the volume of the coin
rate -> the rate at which the order was placed
t_rate -> the trigger rate at which the order was placed
time -> the timestamp at which the order was placed
type -> 1 for sell and 0 for buy order
status -> -1 for cancelled , 0 for not processed , 1 for partially executed, 2 for fully executed
  </pre>
</details>


<b>Get Specify Crypto Coin Address</b><br>
<pre>
Coins Without Tag
bitbnsObj.getCoinAddress('BTC')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
{
  "data": {
    "token": "3QkuWRDRNcjtMQNneoqFV7hpxQPWW6pupK",
    "expiry": "2018-09-12 13:04:09"
  },
  "status": 1,
  "error": null
}

Explanation of fields:
token -> the token address
expiry -> the time till which this address is user's valid address

  </pre>
</details>
<pre>
Coins With Tag
bitbnsObj.getCoinAddress('XLM')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
{
  "data": {
    "token": "GAVQNY45FBHSN5MEPLAF56U7VDCBDG54TQFGJSS2CRPZTWD3CSHP4YPU",
    "tag": "123151"
  },
  "status": 1,
  "error": null
}

Explanation of fields:
token -> the token address
tag -> the tag to be used for the token
Deposits would not be valid unless you specify the tag
  </pre>
</details>

<b>Place Sell Order</b><br>
<pre>bitbnsObj.placeSellOrder('XRP', 200, 25)
200 -> Quantity
25 -> Rate
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
  {
  "data": "Successfully placed bid to sell at specified price",
  "status": 1,
  "error": null,
  "id": 489
}

Explanation of fields:
data -> Just a custom message
id -> the unique id of the order
  </pre>
</details>

<b>Place Buy Order</b><br>
<pre>bitbnsObj.placeBuyOrder('XRP', 200, 25)
200 -> Quantity
25 -> Rate
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
  {
  "data": "Successfully placed bid to purchase currency",
  "status": 1,
  "error": null,
  "id": 490
}

Explanation of fields:
data -> Just a custom message
id -> the unique id of the order
  </pre>
</details>
<b>Placing a STOP LOSS order (BUY)</b><br>
<pre>
bitbnsObj.buyStopLoss('XRP', 40, 24, 24.5)

40 -> Quantity
24 -> Rate
24.5 -> Trigger rate
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
  {
  "data": "Successfully placed order for stop loss buy",
  "status": 1,
  "error": null,
  "id": 28595
}

Explanation of fields:
data -> Just a custom message
id -> the unique id of the order
  </pre>
</details>

<b>Placing a STOP LOSS order (SELL)</b><br>
<pre>
bitbnsObj.sellStopLoss('XRP', 40, 25, 24.5)

40 -> Quantity
24 -> Rate
24.5 -> Trigger rate
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": "Successfully placed a stop limit sell order",
  "status": 1,
  "error": null,
  "id": 28596
}

Explanation of fields:
data -> Just a custom message
id -> the unique id of the order
  </pre>
</details>

<b>Place Cancel Order</b><br>
<pre>bitbnsObj.cancelOrder('XRP', 174)
Here 174 is a order id
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": "Successfully cancelled the order",
  "status": 1,
  "error": null
}

Explanation of fields:
data -> just a custom message
status -> status of cancellation 1 for success
  </pre>
</details>

<b>Getting Sell Order Book for BTC</b><br>
<pre>
bitbnsObj.getSellOrderBook('BTC')
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  data: [
    {
      rate: 481847.56,
      btc: 6352679
    },
    {
      rate: 481700,
      btc: 5540000
    },
    {
      rate: 481551,
      btc: 5000000
    },
    {
      rate: 481000,
      btc: 11406
    },
    {
      rate: 480000,
      btc: 208021
    },
    {
      rate: 479366.65,
      btc: 5265026
    },
    {
      rate: 479345,
      btc: 453445
    },
    {
      rate: 478854.18,
      btc: 642042
    },
    {
      rate: 478749.87,
      btc: 208356
    },
    {
      rate: 478511.87,
      btc: 2446067
    },
    {
      rate: 478000,
      btc: 80253706
    },
    {
      rate: 477900,
      btc: 6261808
    },
    {
      rate: 477777,
      btc: 208900000
    },
    {
      rate: 477740,
      btc: 15000000
    },
    {
      rate: 477706.19,
      btc: 5003424
    }
  ],
  status: 1,
  error: null
}

 Explanation of fields:
 rate -> the amount of the order
 btc -> the volume of the coin for that order
   </pre>
</details>

<b>Getting Sell Order Book for BTCUSDT</b><br>
<pre>
bitbnsObj.getSellOrderBook('BTCUSDT')
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
    "data": [
        { "rate": 13701.34, "btc": 0.145853 },
        { "rate": 13701.35, "btc": 0.043633 },
        { "rate": 13701.47, "btc": 0.543258 },
        { "rate": 13701.69, "btc": 0.664955 },
        { "rate": 13701.72, "btc": 0.131749 },
        { "rate": 13702.36, "btc": 0.406614 },
        { "rate": 13703.18, "btc": 0.253289 },
        { "rate": 13713.46, "btc": 0.19549 },
        { "rate": 13713.88, "btc": 0.055847 },
        { "rate": 13740, "btc": 0.03642294 },
        { "rate": 13848.3, "btc": 0.14447299 },
        { "rate": 13855, "btc": 0.03 },
        { "rate": 13855.11, "btc": 0.0119887 },
        { "rate": 13879.39, "btc": 0.0001 },
        { "rate": 14000, "btc": 0.00163832 }
    ],
    "status": 1,
    "error": None,
    "code": 200
}


 Explanation of fields:
 rate -> the amount of the order
 btc -> the volume of the coin for that order
   </pre>
</details>

<b>Getting Buy Order Book for BTC</b><br>
<pre>
bitbnsObj.getBuyOrderBook('BTC')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    { data:
  [ { rate: 481847.56, btc: 6352679 },
    { rate: 481700, btc: 5540000 },
    { rate: 481551, btc: 5000000 },
    { rate: 481000, btc: 11406 },
    { rate: 480000, btc: 208021 },
    { rate: 479366.65, btc: 5265026 },
    { rate: 479345, btc: 453445 },

    { rate: 478854.18, btc: 642042 },
    { rate: 478749.87, btc: 208356 },
    { rate: 478511.87, btc: 2446067 },
    { rate: 478000, btc: 80253706 },
    { rate: 477900, btc: 6261808 },
    { rate: 477777, btc: 208900000 },
    { rate: 477740, btc: 15000000 },
    { rate: 477706.19, btc: 5003424 } ],
 status: 1,
 error: null }

 Explanation of fields:
 rate -> the amount of the order
 btc -> the volume of the coin for that order
  </pre>
</details>

<b>Getting Buy Order Book for BTCUSDT</b><br>
<pre>
bitbnsObj.getBuyOrderBook('BTCUSDT')
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
    "data": [
        { "rate": 13657.14, "btc": 0.245901 },
        { "rate": 13656.94, "btc": 0.043868 },
        { "rate": 13656.58, "btc": 0.249137 },
        { "rate": 13656.57, "btc": 0.215321 },
        { "rate": 13656.56, "btc": 0.06557399 },
        { "rate": 13656.26, "btc": 0.28264299 },
        { "rate": 13621.07, "btc": 0.086085 },
        { "rate": 13620.93, "btc": 0.307243 },
        { "rate": 13620.77, "btc": 0.466551 },
        { "rate": 13620.71, "btc": 0.203805 },
        { "rate": 13618.79, "btc": 0.01179179 },
        { "rate": 13600, "btc": 0.00461852 },
        { "rate": 13150, "btc": 0.07585551 },
        { "rate": 13000, "btc": 0.00368308 },
        { "rate": 12950, "btc": 0.01540463 }
    ],
    "status": 1,
    "error": None,
    "code": 200
}


 Explanation of fields:
 rate -> the amount of the order
 btc -> the volume of the coin for that order
  </pre>
</details>

<b>Get API usage Status</b><br>
<pre>
bitbnsObj.getApiUsageStatus()
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
     data: {
        readLimt : 100,
        writeLimit : 30,
        readRateUsed: 0,
        writeRateUsed: 1,
        status: 1
     },
      status: 1,
      error: null
    }

  Explanation of the fields:
  readLimit -> the read limit of the user
  writeLimit -> the write limit of the user
  readRateUsed -> the read requests used
  writeRateUsed -> the write requests used
  </pre>
</details>

<b>Getting Order Status</b><br>
<pre>
bitbnsObj.orderStatus('BTC', '4221')
4221 -> order id
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
{
  data: [
    {
      entry_id: 4221,
      btc: 0.001,
      rate: 306929.01,
      time: '2018-09-20T13:54:21.000Z',
      type: 0,
      status: 0
    }
  ],
  status: 1,
  error: null
}

Explanation of fields:
entry_id -> the unique id for the order
btc -> the volume of the currency placed
rate -> the rate at which the order is placed
time -> the timestamp of the entry
type -> 0 for buy and 1 for sell
status -> -1 for cancelled, 0 for not processed, 1 for partially executed, 2 for fully executed
  </pre>
</details>

<b>Cancel Stop Loss Order</b><br>
<pre>
bitbnsObj.cancelStopLossOrder('BTC', 4221)
4221 -> order id
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  data: 'Successfully cancelled the order',
  status: 1,
  error: null
}

Explanation of fields:
data -> the custom message
status -> for successful request the status is 1
  </pre>
</details>


<b>Curl request to get server time</b><br>

<pre>

curl -H "X-BITBNS-APIKEY: API-KEY" -X GET 'https://api.bitbns.com/api/trade/v1/getServerTime'
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  serverTime: '1538150764273',
  status: 1,
  error: null
}

Explanation of fields:
serverTime -> the server timestamp
status -> the response succeeded
  </pre>
</details>

<h3>API V2 (New Features)</h3>
<b>Place Orders(BUY or SELL)</b><br>
<pre>
<b>(Placing Bracket Order)</b>

bitbnsObj.placeOrders({'symbol': 'XRP', 'side': 'BUY', 'quantity': 40, 'rate': 4, 'target_rate': 5, 't_rate': 3.5, 'trail_rate': .01})

side -> BUY or SELL
symbol -> COIN NAME,
quantity -> QUANTITY,
rate -> RATE,
target_rate -> TARGET RATE,
t_rate -> TRRIGER RATE,
trail_rate -> TRAIL RATE

To Place Simple Buy or Sell Order use <b>rate</b>
To Place Stoploss Buy or Sell Order use <b>rate & t_rate</b>
To Place Bracket Buy or Sell Order use <b>rate , t_rate, target_rate & trail_rate</b>
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": "Successfully placed a bracket order",
  "status": 1,
  "error": null,
  "id": 4518726,
  "code": 200
}

Explanation of fields:
data -> the custom message
status -> for successful request the status is 1
id -> the unique id of the order
  </pre>
</details>

<b>Cancel Order</b><br>
<pre>
bitbnsObj.cancelOrders({'symbol': 'XRP', 'side' : 'cancelOrder', 'entry_id': 462})

side -> "cancelOrder","cancelStopLossOrder", "usdtcancelOrder", "usdtcancelStopLossOrder"
symbol -> COIN NAME
entry_id : ENTRY ID
</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": "Successfully cancelled the order",
  "status": 1,
  "error": null,
  "code": 200
}

Explanation of fields:
data -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<b>Place Orders in USDT Market</b><br>
<pre>
bitbnsObj.placeOrders({'symbol': 'TRX_USDT', 'side': 'BUY', 'quantity': 40, 'rate': 4, 'target_rate': 5, 't_rate': 3.5, 'trail_rate': .01})

side -> BUY or SELL
symbol -> COIN NAME(use suffix "_USDT" with coin name)
quantity -> QUANTITY,
rate -> RATE,
target_rate -> TARGET RATE,
t_rate -> TRRIGER RATE,
trail_rate -> TRAIL RATE

To Place Simple Buy or Sell Order use <b>rate</b>
To Place Stoploss Buy or Sell Order use <b>rate & t_rate</b>
To Place Bracket Buy or Sell Order use <b>rate , t_rate, target_rate & trail_rate</b>
</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
   {
  "data": "Successfully placed bid to purchase currency",
  "status": 1,
  "error": null,
  "id": 6743385,
  "code": 200
}

Explanation of fields:
data -> the custom message
status -> for successful request the status is 1
id -> the unique id of the order
  </pre>
</details>

<b>Cancel Order in USDT MARKET</b><br>
<pre>

bitbnsObj.cancelOrders({'symbol': 'TRX_USDT', 'side' : 'usdtcancelOrder', 'entry_id': 462})

side -> "cancelOrder","cancelStopLossOrder", "usdtcancelOrder", "usdtcancelStopLossOrder"
symbol -> COIN NAME(use suffix "_USDT" with coin name)
entry_id : ENTRY ID

</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": "Successfully cancelled the order",
  "status": 1,
  "error": null,
  "code": 200
}

Explanation of fields:
data -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<b>Get Orders in USDT MARKET</b><br>
<pre>

bitbnsObj.getOrders({'side' : 'usdtListOpenOrders', 'symbol' : 'TRX_USDT', 'page' : 0})

side -> "listOpenOrders", "listOpenStopOrders", "listOpenBracketOrders", "usdtListOpenBracketOrders",
         "usdtListOpenStopOrders","usdtListOpenOrders"
symbol -> COIN NAME(use suffix "_USDT" with coin name)
page -> INTEGER

</pre>
<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": [
    {
      "entry_id": 6747351,
      "btc": 750,
      "rate": 0.02,
      "time": "2020-10-31T04:43:30.000Z",
      "type": 0,
      "status": 0
    }
  ],
  "status": 1,
  "error": null,
  "code": 200
}

Explanation of fields:
rate -> the amount of the order
btc -> the volume of the coin for that order
type -> 1 for sell and 0 for buy order
status -> for successful request the status is 1
  </pre>
</details>

<b>Margin Trading V2 APIs</b><br>
<pre>
<b>Place a margin order</b>

bitbnsObj.placeMarginOrders({'symbol': 'USDT', 'side': 'placeOrder', 'type': 'LEND', 'qnty': 40, 'days': 1, 'rate': 0.0055})

side -> placeOrder
type -> BORROW or LEND
days -> 1,3,7,15,30
renew -> 0,1,2
symbol -> COIN NAME,
qnty -> QUANTITY,
rate -> RATE

Renew Flags => 0 - Don't renew, 1 -> Renew only Principal, 2 -> Renew with Principal + Interest

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "status": 1,
  "error": "Successfully placed lend order for Margin trading.",
  "code": 200
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Cancel a margin order</b>

bitbnsObj.cancelMarginOrder({'id': 1, 'side': 'cancelMarginOrder', 'symbol': 'USDT'})

Pass id of the margin transaction you are looking to cancel
symbol -> COIN NAME,

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
      "status": 1,
      "error": "Successfully cancelled the order",
      "code": 200
    }

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Settle a margin order partially</b>

bitbnsObj.settleMarginPartial({'id': 1, 'side': 'settleMarginOrderPartial', 'amt': 50, 'symbol': 'USDT'})

amt -> Amount to settle

Pass id of the margin transaction you are looking to settle and amt you want to settle

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "status": 1,
  "error": "Successfully settled the margin order",
  "code": 200
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Settle a margin order completely</b>

bitbnsObj.settleMargin({ 'id' : 1, 'side' : 'settleMarginOrder', 'symbol': 'USDT' })

Pass id of the margin transaction you are looking to settle

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "status": 1,
  "error": "Successfully settled the margin order",
  "code": 200
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Get my margin executed orders</b>

bitbnsObj.listMarginExecuted({'page': 1, 'side': 'listMarginExecuted', 'type': 'BORROW', 'symbol': 'USDT'})

type => LEND or BORROW

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
  response for borrow:
  {
    "data": [
      {
        "entry_id": 53298,
        "worth_required": 8129.82,
        "worth_current": 26779.7,
        "margin_taken": 85,
        "status": 0,
        "expiry": "2020-11-01T07:03:04.000Z",
        "phase": 0,
        "margin_to_return": 85.04,
        "days": 1,
        "interest": 0.055,
        "coin": 54,
        "margin_partial_return": 0
      }
    ],
    "status": 1,
    "error": null,
    "code": 200
  }
response for lend:
    {
      "data": [
        {
          "entry_id": 114143,
          "amt": 50,
          "time": "2020-02-03T02:48:41.000Z",
          "status": 10,
          "expiry": "2020-02-18T08:18:41.000Z",
          "days": 15,
          "interest": 0.051,
          "coin": 54,
          "renew": 0
        }
      ],
      "status": 1,
      "error": null,
      "code": 200
    }

Explanation of fields:
data -> the custom message
worth_required -> the amount required to maintain the margin
worth_current -> current worth of margin borrwoed
margin_taken -> the amount value borrowed
expiry -> time of expiry of margin
margin_to_return -> amount to be returned.
days -> number of days the margin was borrowed or lent.
interest -> intreset of margin per day.
amt -> the amount of coins lent
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Get my margin pending orders</b>

bitbnsObj.listMarginPending({'page': 1, 'side': 'listMarginPending', 'symbol': 'USDT'})

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": [
    {
      "entry_id": 215769,
      "btc": 40,
      "days": 1,
      "time": "2020-10-31T06:42:54.000Z",
      "type": 0,
      "status": 0,
      "rate": 0.083
    }
  ],
  "status": 1,
  "error": null,
  "code": 200
}

Explanation of fields:
data -> the custom message
entry_id -> the unique id assigned to the order
days -> number of days lent or borrowed
btc -> the volume of the coin
type -> 1 for borrow and 0 for lend order
rate -> the rate at which the margin is lend or borrowed
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Get open orders of margin market - all users</b>

bitbnsObj.listMarginMarketOrders({'type': 'BORROW', 'side': 'listMarketOrders', 'symbol': 'XRP'})

type => LEND or BORROW

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
  "data": [
    {
      "btc": 486.55,
      "days": 7,
      "rate": 0.0539
    },
    {
      "btc": 2.31,
      "days": 1,
      "rate": 0.055
    },
    {
      "btc": 4392.95,
      "days": 3,
      "rate": 0.06
    },
    {
      "btc": 99.96,
      "days": 15,
      "rate": 0.065
    },
    {
      "btc": 1242,
      "days": 30,
      "rate": 0.065
    },
    {
      "btc": 13287.65,
      "days": 7,
      "rate": 0.067
    },
    {
      "btc": 350,
      "days": 30,
      "rate": 0.068
    },
    {
      "btc": 5500,
      "days": 7,
      "rate": 0.07
    },
    {
      "btc": 2119.34,
      "days": 30,
      "rate": 0.0749
    },
    {
      "btc": 1770.51,
      "days": 30,
      "rate": 0.076
    },
    {
      "btc": 53.52,
      "days": 30,
      "rate": 0.0779
    },
    {
      "btc": 3231.92,
      "days": 15,
      "rate": 0.078
    },
    {
      "btc": 622.69,
      "days": 15,
      "rate": 0.079
    },
    {
      "btc": 17306,
      "days": 1,
      "rate": 0.08
    },
    {
      "btc": 7840,
      "days": 15,
      "rate": 0.085
    },
    {
      "btc": 446.07,
      "days": 30,
      "rate": 0.0855
    },
    {
      "btc": 762.59,
      "days": 30,
      "rate": 0.0856
    },
    {
      "btc": 500,
      "days": 30,
      "rate": 0.087
    },
    {
      "btc": 195.66,
      "days": 30,
      "rate": 0.088
    },
    {
      "btc": 112.33,
      "days": 30,
      "rate": 0.089
    },
    {
      "btc": 2769,
      "days": 1,
      "rate": 0.09
    },
    {
      "btc": 20000,
      "days": 3,
      "rate": 0.09
    },
    {
      "btc": 7000,
      "days": 7,
      "rate": 0.09
    },
    {
      "btc": 8525.51,
      "days": 30,
      "rate": 0.09
    },
    {
      "btc": 206,
      "days": 1,
      "rate": 0.091
    },
    {
      "btc": 20000,
      "days": 15,
      "rate": 0.091
    },
    {
      "btc": 2096.32,
      "days": 30,
      "rate": 0.099
    },
    {
      "btc": 235,
      "days": 1,
      "rate": 0.1
    },
    {
      "btc": 401780.26,
      "days": 30,
      "rate": 0.1
    },
    {
      "btc": 50000,
      "days": 30,
      "rate": 0.11
    },
    {
      "btc": 19999.81,
      "days": 15,
      "rate": 0.12
    },
    {
      "btc": 61.71,
      "days": 30,
      "rate": 0.12
    },
    {
      "btc": 107.45,
      "days": 30,
      "rate": 0.14
    },
    {
      "btc": 43212,
      "days": 15,
      "rate": 0.169
    },
    {
      "btc": 30000,
      "days": 7,
      "rate": 0.17
    },
    {
      "btc": 90610.26,
      "days": 30,
      "rate": 0.18
    }
  ],
  "status": 1,
  "error": null,
  "code": 200
}

Explanation of fields:
data -> the custom message
days -> number of days lent or borrowed
btc -> the volume of the coin
rate -> the rate at which the margin is lend or borrowed
status -> for successful request the status is 1
  </pre>
</details>

--------

## **__Options Trading APIs__**

<pre>
<b>List all options instruments</b>

bitbnsObj.listAllInstruments()

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
      "msg": "List of instruments",
      "status": 1,
      "code": 200,
      "data": {
        "BTC-8JAN21-23500-C": "1360",
        "BTC-8JAN21-22000-C": "1362",
        "BTC-8JAN21-27000-P": "1369",
        "BTC-8JAN21-19000-P": "1370",
        "BTC-8JAN21-22000-P": "1371",
        "BTC-8JAN21-24000-P": "1372",
        "BTC-8JAN21-29000-P": "1374",
        "BTC-8JAN21-30000-P": "1376",
        "BTC-8JAN21-23000-C": "1377",
        "BTC-8JAN21-26500-P": "1378",
        "BTC-8JAN21-23000-P": "1379",
        "BTC-8JAN21-21500-P": "1380",
        "BTC-8JAN21-28500-C": "1383",
        "BTC-8JAN21-24500-P": "1384",
        "BTC-8JAN21-28000-P": "1388",
        "BTC-8JAN21-29500-C": "1390",
        "BTC-8JAN21-21000-P": "1393",
        "BTC-8JAN21-28500-P": "1397",
        "BTC-8JAN21-30000-C": "1398",
        "BTC-8JAN21-29000-C": "1399",
        "BTC-8JAN21-22500-P": "1403",
        "BTC-8JAN21-24500-C": "1407",
        "BTC-8JAN21-21000-C": "1409",
        "BTC-8JAN21-19500-P": "1411",
        "BTC-8JAN21-26500-C": "1412",
        "BTC-8JAN21-25500-C": "1413",
        "BTC-8JAN21-27000-C": "1417",
        "BTC-8JAN21-29500-P": "1418",
        "BTC-8JAN21-27500-C": "1419",
        "BTC-8JAN21-23500-P": "1420",
        "BTC-8JAN21-21500-C": "1423",
        "BTC-8JAN21-19500-C": "1426",
        "BTC-8JAN21-25000-C": "1428",
        "BTC-8JAN21-28000-C": "1429",
        "BTC-8JAN21-26000-C": "1431",
        "BTC-8JAN21-20000-C": "1433",
        "BTC-8JAN21-24000-C": "1434",
        "BTC-8JAN21-25500-P": "1435",
        "BTC-8JAN21-20000-P": "1436",
        "BTC-8JAN21-25000-P": "1440",
        "BTC-8JAN21-20500-P": "1441",
        "BTC-8JAN21-19000-C": "1442",
        "BTC-8JAN21-20500-C": "1444",
        "BTC-8JAN21-26000-P": "1445",
        "BTC-8JAN21-22500-C": "1447",
        "BTC-8JAN21-27500-P": "1448",
        "BTC-8JAN21-30500-C": "1454",
        "BTC-8JAN21-30500-P": "1456",
        "BTC-8JAN21-31000-P": "1459",
        "BTC-8JAN21-31000-C": "1461",
        "BTC-8JAN21-31500-P": "1472",
        "BTC-8JAN21-31500-C": "1473",
        "BTC-8JAN21-33000-C": "1478",
        "BTC-8JAN21-32000-P": "1480",
        "BTC-8JAN21-32000-C": "1481",
        "BTC-8JAN21-33000-P": "1482",
        "BTC-8JAN21-34000-C": "1486",
        "BTC-8JAN21-36000-C": "1487",
        "BTC-8JAN21-34000-P": "1491",
        "BTC-8JAN21-36000-P": "1492",
        "BTC-8JAN21-40000-P": "1497",
        "BTC-8JAN21-40000-C": "1498",
        "BTC-8JAN21-16000-P": "1511",
        "BTC-8JAN21-16000-C": "1515",
        "BTC-8JAN21-18000-C": "1521",
        "BTC-8JAN21-18000-P": "1522",
        "BTC-15JAN21-28000-P": "1766",
        "BTC-15JAN21-20000-P": "1772",
        "BTC-15JAN21-24000-P": "1773",
        "BTC-15JAN21-28000-C": "1774",
        "BTC-15JAN21-22000-P": "1775",
        "BTC-15JAN21-32000-P": "1778",
        "BTC-15JAN21-22000-C": "1779",
        "BTC-15JAN21-32000-C": "1781",
        "BTC-15JAN21-30000-C": "1784",
        "BTC-15JAN21-20000-C": "1785",
        "BTC-15JAN21-30000-P": "1786",
        "BTC-15JAN21-34000-C": "1792",
        "BTC-15JAN21-26000-P": "1793",
        "BTC-15JAN21-34000-P": "1794",
        "BTC-15JAN21-24000-C": "1803",
        "BTC-15JAN21-26000-C": "1814",
        "BTC-15JAN21-23000-C": "1873",
        "BTC-15JAN21-27000-C": "1874",
        "BTC-15JAN21-21000-P": "1875",
        "BTC-15JAN21-25000-P": "1876",
        "BTC-15JAN21-29000-P": "1877",
        "BTC-15JAN21-23000-P": "1878",
        "BTC-15JAN21-21000-C": "1879",
        "BTC-15JAN21-29000-C": "1880",
        "BTC-15JAN21-25000-C": "1881",
        "BTC-15JAN21-27000-P": "1882",
        "BTC-15JAN21-36000-C": "1883",
        "BTC-15JAN21-36000-P": "1884",
        "BTC-15JAN21-38000-C": "1943",
        "BTC-15JAN21-38000-P": "1944",
        "BTC-8JAN21-38000-C": "2007",
        "BTC-15JAN21-40000-C": "2008",
        "BTC-8JAN21-38000-P": "2009",
        "BTC-15JAN21-40000-P": "2010",
        "BTC-29JAN21-17000-C": "2131",
        "BTC-29JAN21-8000-C": "2132",
        "BTC-29JAN21-10000-P": "2133",
        "BTC-29JAN21-8000-P": "2134",
        "BTC-29JAN21-20000-C": "2135",
        "BTC-29JAN21-18000-C": "2136",
        "BTC-29JAN21-10000-C": "2137",
        "BTC-29JAN21-34000-C": "2138",
        "BTC-29JAN21-22000-P": "2139",
        "BTC-29JAN21-34000-P": "2140",
        "BTC-29JAN21-27000-P": "2141",
        "BTC-29JAN21-24000-P": "2142",
        "BTC-29JAN21-25000-C": "2143",
        "BTC-29JAN21-16000-P": "2144",
        "BTC-29JAN21-25000-P": "2145",
        "BTC-29JAN21-28000-P": "2146",
        "BTC-29JAN21-32000-P": "2147",
        "BTC-29JAN21-23000-C": "2148",
        "BTC-29JAN21-21000-C": "2149",
        "BTC-29JAN21-26000-P": "2150",
        "BTC-29JAN21-19000-P": "2151",
        "BTC-29JAN21-12000-P": "2152",
        "BTC-29JAN21-30000-P": "2153",
        "BTC-29JAN21-18000-P": "2154",
        "BTC-29JAN21-16000-C": "2155",
        "BTC-29JAN21-24000-C": "2156",
        "BTC-29JAN21-23000-P": "2157",
        "BTC-29JAN21-44000-C": "2158",
        "BTC-29JAN21-28000-C": "2159",
        "BTC-29JAN21-22000-C": "2160",
        "BTC-29JAN21-52000-C": "2161",
        "BTC-29JAN21-17000-P": "2162",
        "BTC-29JAN21-40000-P": "2163",
        "BTC-29JAN21-52000-P": "2164",
        "BTC-29JAN21-20000-P": "2165",
        "BTC-29JAN21-27000-C": "2166",
        "BTC-29JAN21-36000-C": "2167",
        "BTC-29JAN21-36000-P": "2168",
        "BTC-29JAN21-19000-C": "2169",
        "BTC-29JAN21-14000-P": "2170",
        "BTC-29JAN21-12000-C": "2171",
        "BTC-29JAN21-48000-P": "2172",
        "BTC-29JAN21-48000-C": "2173",
        "BTC-29JAN21-21000-P": "2174",
        "BTC-29JAN21-14000-C": "2175",
        "BTC-29JAN21-32000-C": "2176",
        "BTC-29JAN21-44000-P": "2177",
        "BTC-29JAN21-26000-C": "2178",
        "BTC-29JAN21-30000-C": "2179",
        "BTC-29JAN21-40000-C": "2180",
        "BTC-22JAN21-26000-P": "2182",
        "BTC-15JAN21-31000-P": "2186",
        "BTC-22JAN21-30000-P": "2188",
        "BTC-22JAN21-38000-C": "2191",
        "BTC-22JAN21-31000-P": "2193",
        "BTC-15JAN21-33000-P": "2194",
        "BTC-22JAN21-32000-P": "2195",
        "BTC-22JAN21-42000-P": "2197",
        "BTC-22JAN21-24000-C": "2198",
        "BTC-22JAN21-42000-C": "2202",
        "BTC-22JAN21-40000-C": "2204",
        "BTC-22JAN21-27000-C": "2205",
        "BTC-22JAN21-26000-C": "2208",
        "BTC-22JAN21-40000-P": "2215",
        "BTC-22JAN21-31000-C": "2217",
        "BTC-22JAN21-29000-P": "2218",
        "BTC-22JAN21-34000-C": "2219",
        "BTC-22JAN21-28000-C": "2222",
        "BTC-22JAN21-28000-P": "2224",
        "BTC-22JAN21-33000-P": "2225",
        "BTC-22JAN21-38000-P": "2227",
        "BTC-22JAN21-36000-P": "2229",
        "BTC-22JAN21-29000-C": "2232",
        "BTC-22JAN21-25000-P": "2233",
        "BTC-15JAN21-33000-C": "2234",
        "BTC-15JAN21-31000-C": "2238",
        "BTC-22JAN21-32000-C": "2241",
        "BTC-22JAN21-25000-C": "2246",
        "BTC-22JAN21-33000-C": "2247",
        "BTC-22JAN21-30000-C": "2251",
        "BTC-22JAN21-36000-C": "2253",
        "BTC-22JAN21-34000-P": "2256",
        "BTC-22JAN21-24000-P": "2258",
        "BTC-22JAN21-27000-P": "2262",
        "BTC-22JAN21-22000-P": "2265",
        "BTC-22JAN21-22000-C": "2266",
        "BTC-22JAN21-48000-C": "2417",
        "BTC-15JAN21-44000-P": "2418",
        "BTC-22JAN21-44000-P": "2419",
        "BTC-15JAN21-44000-C": "2420",
        "BTC-22JAN21-48000-P": "2421",
        "BTC-22JAN21-44000-C": "2422",
        "BTC-29JAN21-56000-C": "2423",
        "BTC-29JAN21-56000-P": "2424",
        "BTC-8JAN21-44000-C": "2425",
        "BTC-8JAN21-44000-P": "2426",
        "BTC-15JAN21-48000-P": "2427",
        "BTC-15JAN21-48000-C": "2428",
        "BTC-22JAN21-52000-P": "2431",
        "BTC-22JAN21-52000-C": "2432",
        "BTC-6JAN21-36000-P": "2477",
        "BTC-6JAN21-32500-C": "2478",
        "BTC-6JAN21-31000-P": "2479",
        "BTC-6JAN21-34000-C": "2480",
        "BTC-6JAN21-32000-C": "2481",
        "BTC-6JAN21-30500-C": "2482",
        "BTC-6JAN21-32000-P": "2483",
        "BTC-6JAN21-29000-C": "2484",
        "BTC-6JAN21-31000-C": "2485",
        "BTC-6JAN21-35500-C": "2486",
        "BTC-6JAN21-34500-P": "2487",
        "BTC-6JAN21-33000-P": "2488",
        "BTC-6JAN21-29000-P": "2489",
        "BTC-6JAN21-35500-P": "2490",
        "BTC-6JAN21-36000-C": "2491",
        "BTC-6JAN21-35000-P": "2492",
        "BTC-6JAN21-31500-C": "2493",
        "BTC-6JAN21-34500-C": "2494",
        "BTC-6JAN21-30500-P": "2495",
        "BTC-6JAN21-33500-P": "2496",
        "BTC-6JAN21-33000-C": "2497",
        "BTC-6JAN21-33500-C": "2498",
        "BTC-6JAN21-34000-P": "2499",
        "BTC-6JAN21-30000-P": "2500",
        "BTC-6JAN21-29500-C": "2501",
        "BTC-6JAN21-31500-P": "2502",
        "BTC-6JAN21-30000-C": "2503",
        "BTC-6JAN21-29500-P": "2504",
        "BTC-6JAN21-32500-P": "2505",
        "BTC-6JAN21-35000-C": "2506",
        "BTC-6JAN21-28500-P": "2507",
        "BTC-6JAN21-28500-C": "2508",
        "BTC-6JAN21-28000-P": "2511",
        "BTC-6JAN21-28000-C": "2512",
        "BTC-6JAN21-27500-P": "2515",
        "BTC-6JAN21-27500-C": "2516",
        "BTC-6JAN21-26000-C": "2518",
        "BTC-6JAN21-26000-P": "2520",
        "BTC-6JAN21-27000-P": "2521",
        "BTC-6JAN21-26500-C": "2524",
        "BTC-22JAN21-20000-C": "2527",
        "BTC-6JAN21-27000-C": "2528",
        "BTC-6JAN21-25500-P": "2529",
        "BTC-22JAN21-20000-P": "2530",
        "BTC-6JAN21-25500-C": "2532",
        "BTC-6JAN21-26500-P": "2533",
        "BTC-7JAN21-34000-C": "2535",
        "BTC-7JAN21-33500-P": "2536",
        "BTC-7JAN21-29000-P": "2537",
        "BTC-7JAN21-34500-P": "2538",
        "BTC-7JAN21-31000-C": "2539",
        "BTC-7JAN21-29000-C": "2540",
        "BTC-7JAN21-28000-P": "2541",
        "BTC-7JAN21-28500-C": "2542",
        "BTC-7JAN21-33000-P": "2543",
        "BTC-7JAN21-30000-P": "2544",
        "BTC-7JAN21-31500-P": "2545",
        "BTC-7JAN21-33500-C": "2546",
        "BTC-7JAN21-29500-P": "2547",
        "BTC-7JAN21-33000-C": "2548",
        "BTC-7JAN21-28500-P": "2549",
        "BTC-7JAN21-30000-C": "2550",
        "BTC-7JAN21-31500-C": "2551",
        "BTC-7JAN21-32000-P": "2552",
        "BTC-7JAN21-31000-P": "2553",
        "BTC-7JAN21-34500-C": "2554",
        "BTC-7JAN21-32500-P": "2555",
        "BTC-7JAN21-28000-C": "2556",
        "BTC-7JAN21-34000-P": "2557",
        "BTC-7JAN21-30500-P": "2558",
        "BTC-7JAN21-32500-C": "2559",
        "BTC-7JAN21-29500-C": "2560",
        "BTC-7JAN21-30500-C": "2561",
        "BTC-7JAN21-32000-C": "2562",
        "BTC-7JAN21-35000-C": "2563",
        "BTC-7JAN21-35000-P": "2564",
        "BTC-7JAN21-35500-C": "2565",
        "BTC-7JAN21-35500-P": "2566"
  }
}

Explanation of fields:
data -> the custom message
entry_id -> the unique id assigned to the order
days -> number of days lent or borrowed
btc -> the volume of the coin
type -> 1 for borrow and 0 for lend order
rate -> the rate at which the margin is lend or borrowed
status -> for successful request the status is 1
  </pre>
</details>


<pre>
<b>get options wallet balance</b>

bitbnsObj.getOptionsBalance()

Pass id of the margin transaction you are looking to settle

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
      "data":{
          "BTC":{
            "balance":0.9988,
            "inobalance":0,
            "lockbalance":0,
            "freezebalance":0
          }
      },
      "status":1,
      "error":"None",
      "code":200
    }

Explanation of fields:
balance -> total account balance
inobalance -> balance currently held in order at any given time t,
               value updates at every price change.
lockbalance -> balance currently locked for maintainace margin
               and order
freezebalance -> balance currently held, considers maintaince margin
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>


<pre>
<b>Place options BUY/SELL order</b>

bitbnsObj.placeOptionOrder({
        'side': 'BUY',
        'prem': 0.001,
        'qnty': 0.005,
        'instrument': 'BTC-6JAN21-32500-P',
        'symbol': 'BTC'
    })

side -> BUY/SELL
prem -> premium to be paid on the options
qnty -> order volume/quantity
instrument -> name of the instrument
symbol -> symbol of the options market

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
    "status": 1,
    "error": "Successfully placed a buy order",
    "code": 200
  }

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>



<pre>
<b>Get options order details</b>

bitbnsObj.bitbnsObj.listOptionDetails({
    'symbol': 'BTC',
    'side': 'OPEN'
})

side -> OPEN, ORDER, TRADE, POSITION
    OPEN -> get open orders
    ORDER -> get all order history
    TRADE -> get exceuted trade list
    POSITION -> get current options positions
symbol -> symbol of the options market

</pre>

<details>
  <summary>
   View Response - OPEN
  </summary>
  <pre>
    {
   "data":[
      {
         "id":893,
         "ins_id":2505,
         "qnty":0.005,
         "qnty_rem":0.005,
         "prem":0.001,
         "type":0,
         "initial_margin":1e-05,
         "order_time":"2021-01-06T04:08:06.000Z"
      }
   ],
   "status":1,
   "error":"None",
   "code":200
}

Explanation of fields:
id -> order id
ins_id -> instrument id
qnty -> order quanty
qnty_rem -> remaining order quantity
prem -> options premium amount
type -> 0 = BUY, 1 = SELL
initial_margin -> Margin reserved for your open positions and open orders.
                  If your Margin Balance falls below Initial Margin requirements,
                  open orders that would increase your position get cancelled and
                  you will only be able to place orders that reduce your position.
order_time -> time at which order was placed
  </pre>
</details>

<details>
  <summary>
   View Response - ORDER
  </summary>
  <pre>
    {
   "code":200,
   "data":[
      {
         "id":894,
         "initial_margin":7.582e-05,
         "ins_id":2505,
         "order_time":"2021-01-06T05:35:31.000Z",
         "prem":0.001,
         "qnty":0.0055,
         "qnty_rem":0.0005,
         "status":0,
         "type":1
      }
   ],
   "error":"None",
   "status":1
}

Explanation of fields:
id -> order id
initial_margin -> Margin reserved for your open positions and open orders.
                  If your Margin Balance falls below Initial Margin requirements,
                  open orders that would increase your position get cancelled and
                  you will only be able to place orders that reduce your position.
ins_id -> instrument id
order_time -> time at which order was placed
prem -> options premium amount
qnty -> order quanty
qnty_rem -> remaining order quantity
type -> 0 = BUY, 1 = SELL

  </pre>
</details>

<details>
  <summary>
   View Response - TRADE
  </summary>
  <pre>
    {
   "code":200,
   "data":[
      {
         "entry_id":392,
         "id":894,
         "ins_id":2505,
         "prem":0.001,
         "qnty":0.0005,
         "status":1,
         "time":"2021-01-06T11:50:56.193Z",
         "type":1
      }
   ],
   "error":"None",
   "status":1
}

Explanation of fields:
id -> order id
ins_id -> instrument id
time -> time at which order was executed
prem -> options premium amount
qnty -> order quanty
qnty_rem -> remaining order quantity
type -> 0 = BUY, 1 = SELL
  </pre>
</details>

<details>
  <summary>
   View Response - POSITION
  </summary>
  <pre>
    {
   "code":200,
   "data":[
      {
         "avg_price":0.001,
         "init_margin":7.531e-05,
         "ins_id":2505,
         "last_updated":"2021-01-06T05:50:59.000Z",
         "main_margin":3.781e-05,
         "pos_id":198,
         "position":-0.0005
      }
   ],
   "error":"None",
   "status":1
}

Explanation of fields:
avg_price -> average price at the order was filled
initial_margin -> Margin reserved for your open positions and open orders.
                  If your Margin Balance falls below Initial Margin requirements,
                  open orders that would increase your position get cancelled and
                  you will only be able to place orders that reduce your position.
ins_id -> instrument id
last_updated -> time at which status was updated
prem -> options premium amount
pos_id -> id of the psition
position -> current options position.
  </pre>
</details>


<pre>
<b>Cancel options order by order id</b>

bitbnsObj.cancelOptionOrder({
    'order_id': 896,
    'symbol': 'BTC',
    'side': 'INDIVIDUAL'
})


order_id -> order id of the options order
symbol -> symbol of the options market
side -> INDIVIDUAL

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
   "code":200,
   "error":"Successfully cancelled requested order",
   "status":1
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Cancel options order by instrument id</b>

bitbnsObj.cancelOptionOrder({
    'instrument': 'BTC-6JAN21-30000-P',
    'symbol': 'BTC',
    'side': 'INSTRUMENT'
})

instrument -> instrument id of the options
symbol -> symbol of the options market
side -> INSTRUMENT

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
   "code":200,
   "error":"Successfully cancelled requested order",
   "status":1
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

<pre>
<b>Cancel all options orders</b>

bitbnsObj.cancelOptionOrder({
    'symbol': 'BTC',
    'side': 'ALL'
})


symbol -> symbol of the options market
side -> ALL

</pre>

<details>
  <summary>
   View Response
  </summary>
  <pre>
    {
   "code":200,
   "error":"Successfully cancelled requested order",
   "status":1
}

Explanation of fields:
error -> the custom message
status -> for successful request the status is 1
  </pre>
</details>

--------



<h2>HTTP error status codes </h2>
<h3> HTTP error codes would be returned incase of any errors, the body will also cointain an error feild which will explain the cause of the error</h3>
<div id ="HTTP_error_code_table" style ="border:1px solid">
  <table style = "width:100%">
    <tr>
      <th>Code</th>
      <th>Meaning</th>
    </tr>
    <tr>
      <th></th>
      <th></th>
    </tr>
    <tr>
      <th>200</th>
      <th>null -- requested action has been performed without any problems </th>
    </tr>
    <tr>
      <th>400</th>
      <th>Invalid Request -- Invalid request format</th>
    </tr>
    <tr>
      <th>401</th>
      <th>authentication -- Not authorised or invalid API key</th>
    </tr>
    <tr>
      <th>403</th>
      <th>Undefined -- this request is forbidden</th>
    </tr>
    <tr>
      <th>404</th>
      <th>Exchange not found -- Unable to find exchange</th>
    </tr>
    <tr>
      <th>406</th>
      <th>Coin name not supplied or not yet supported -- coin name applied is incorrect</th>
    </tr>
    <tr>
      <th>409</th>
      <th>parameter type not correct -- parameters entered is incorrect</th>
    </tr>
    <tr>
      <th>412</th>
      <th>Oops ! Cancellation failed. Something went wrong ! -- Unable to cancel order</th>
    </tr>
    <tr>
      <th>413</th>
      <th>volume asked not acceptable -- Desired volume is not within bounds</th>
    </tr>
     <tr>
      <th>416</th>
      <th>Oops ! Not sufficient balance to purchase currency -- wallet balance is not sufficient </th>
    </tr>
     <tr>
      <th>417</th>
      <th>Oops ! Order doesn't exist any more -- Order has alredy been deleted</th>
    </tr>
     <tr>
      <th>428</th>
      <th>Price seems Irregular from current market price. -- Entered price is more than current price</th>
    </tr>
         <tr>
      <th>500</th>
      <th>Problem with our servers, try again later</th>
    </tr>
         <tr>
      <th>503</th>
      <th>currently down for maintaince</th>
    </tr>
    </tr>
  </table>
</div>
