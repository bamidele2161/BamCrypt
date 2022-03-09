<template>
  <div class="dashboard-container ">
    <div class="sidebar-container">
        <ul class="sidebar-list">
            <li class="list-item active">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-house"></i>
                    Home
                </router-link>
            </li>
            <li class="list-item">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-wallet"></i>
                    Wallet
                </router-link>
            </li>
            <li class="list-item">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-arrow-trend-up"></i>
                    Live Trade
                </router-link>    
            </li>
            <li class="list-item">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-handshake"></i>
                    Forum
                </router-link>
            </li>
            <li class="list-item">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-right-from-bracket"></i>
                    Reports
                </router-link>
            </li>
            <li class="list-item">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-gear"></i>
                    Settings
                </router-link>
            </li>
            <li class="list-item" id="logout-link">
                <router-link class="side-link" to="/">
                    <i class="fa-solid fa-right-from-bracket"></i>
                    Log Out
                </router-link>
            </li>
        </ul>
    </div>

    <div class="sidepage d-flex justify-between flex-row flex-wrap">
        
        <div class="sidepage-first-item">
            <div class="welcome-div">
                <p class="welcome-greetings">Good Morning, Damiro Emmanuel</p>
                <h3 class="welcome-heading">Check Your Wallet and Smile</h3>
                <p class="regards">Have a good day</p>
            </div>
            <div class="wallet-card-div d-flex justify-content-between flex-row flex-wrap">
                <div class="wallet-card">
                    <div class="balance-currency-name d-flex justify-content-between">
                        <p class="balance">Balance</p>
                        <i class="fa-solid fa-dollar" id="currency-icon"></i>
                    </div>
                    <h3 class="balance-figure">$10,334</h3>
                    <p class="btc-worth">0.3 BTC</p>
                    <div className="arrow-div">
                        <p className="currency-arrow-icon"> &gt; </p>
                    </div>
                </div>

                <div class="wallet-card">
                    <div class="balance-currency-name d-flex justify-content-between">
                        <p class="balance">Today's Profit</p>
                        <i class="fa-solid fa-dollar" id="currency-icon"></i>
                    </div>
                    <h3 class="balance-figure">+$103</h3>
                    <p class="btc-worth">0.0031 BTC</p>
                </div>
            </div>
            <div class="explore-market ">
                <p class="explore-heading">
                    Explore Market
                </p>
                
            </div>
            <div class="explore d-flex justify-content-between flex-row flex-wrap">
                <div class="explore-currency d-flex justify-content-between">
                    <i class="fa-solid fa-dollar" id="currency-explore-icon"></i>
                    <div class="currency-details">
                        <div class="first-row-details d-flex justify-content-between flex-row">
                            <p class="fw-bold">BTC/USDT</p>
                            <P class="currency-current">$37,000</P>
                        </div>
                        <div class="second-details-row d-flex justify-content-between flex-row">
                            <p>Bitcoin</p>
                            <p class="increase-percentage">$503(%2)</p>
                        </div>
                    </div>
                </div>
                <div class="explore-currency d-flex justify-content-between">
                    <i class="fa-solid fa-dollar" id="currency-explore-icon"></i>
                    <div class="currency-details">
                        <div class="first-row-details d-flex justify-content-between flex-row">
                            <p class="fw-bold">ETH/USDT</p>
                            <P class="currency-current">$37,000</P>
                        </div>
                        <div class="second-details-row d-flex justify-content-between flex-row">
                            <p>Bitcoin</p>
                            <p class="increase-percentage">$203(%2)</p>
                        </div>
                    </div>
                </div>
                <div class="explore-currency d-flex justify-content-between">
                    <i class="fa-solid fa-dollar" id="currency-explore-icon"></i>
                    <div class="currency-details">
                        <div class="first-row-details d-flex justify-content-between flex-row">
                            <p class="fw-bold">BNB/USDT</p>
                            <P class="currency-current">$401</P>
                        </div>
                        <div class="second-details-row d-flex justify-content-between flex-row">
                            <p>Bitcoin</p>
                            <p class="increase-percentage">$3(%3)</p>
                        </div>
                    </div>
                </div>
                <div class="explore-currency d-flex justify-content-between">
                    <i class="fa-solid fa-dollar" id="currency-explore-icon"></i>
                    <div class="currency-details">
                        <div class="first-row-details d-flex justify-content-between flex-row">
                            <p class="fw-bold">SOL/USDT</p>
                            <P class="currency-current">$130</P>
                        </div>
                        <div class="second-details-row d-flex justify-content-between flex-row">
                            <p>Bitcoin</p>
                            <p class="increase-percentage">$8(%2)</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="sidebar-second-item">
            <div class="right-first-div">
                <div class="option-div d-flex justify-content-center text-center flex-column">
                    <div v-if="!isSwitched">
                        <div class="trade-nav d-flex justify-content-between">
                            <p class="buy font-weight-bold" @click="buy()">Buy</p>
                            <p class="sell font-weight-bold" @click="sell()">Sell</p>
                        </div>
                        <p class="bit-price">Bitcoin Price</p>
                        <h3 class="bit-price-figure">
                            $39,634
                        </h3>
                        <select name="" id="" class="select-coin">
                            <option value="">BTC</option>
                            <option value="">ETH</option>
                            <option value="">BNB</option>
                            <option value="">AXS</option>
                            <option value="">SOL</option>
                        </select>
                        <input type="text" class="input-amount" placeholder="USDT" />
                        <button class="buy-btn btn-sm">Buy USDT</button>
                    </div>
                
                <div v-if="isSwitched">
                        <div class="trade-nav d-flex justify-content-between">
                            <p class="buy font-weight-bold" @click="buy()">Buy</p>
                            <p class="sell font-weight-bold" @click="sell()">Sell</p>
                        </div>
                        <p class="bit-price">Bitcoin Price</p>
                        <h3 class="bit-price-figure">
                            $39,634
                        </h3>
                        <select name="" id="" class="select-coin">
                            <option value="">BTC</option>
                            <option value="">ETH</option>
                            <option value="">BNB</option>
                            <option value="">AXS</option>
                            <option value="">SOL</option>
                        </select>
                        <input type="text" class="input-amount" placeholder="USDT" />
                        <button class="sell-btn btn-sm">Sell USDT</button>
                </div>

                </div>


                <div class="profile-div d-flex justify-content-center text-center flex-column">
                    <p class="trader-profile">Trader Profile</p>
                    <h1 class="trader-image">D</h1>
                    <p class="trader-name">Damiro Emmanuel</p>
                    <router-link to="/" class="edit-link">Edit Profile</router-link>
                    <p class="account">Account</p>
                    <div class="joined-date d-flex justify-content-between">
                        <p class="joined">Joined</p>
                        <p class="date">January 23, 2022</p>
                    </div>
                    <div class="assets-total d-flex justify-content-between">
                        <p class="joined">Assets Total</p>
                        <p class="asset-figure">$10,331</p>
                    </div>
                    <div class="btn-group">
                        <button id="more-btn" class="btn-secondary btn-sm dropdown-toggle" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            More
                        </button>
                        <div class="dropdown-menu">
                            Withdraw
                        </div>
                    </div>
                </div>
            </div>


            <p class="transaction-history">Transaction History</p>
            <div class="right-second-div d-flex justify-content-between flex-column">
                <div class="trans-history d-flex justify-content-between">
                    <p>22.02.15</p>
                    <p class="fw-bold" id="trans-pair">BTC/USDT</p>
                    <div class="b">
                        <i class="fa-brands fa-bitcoin" ></i><span>0.002</span>
                    </div>
                    <div class="d">
                        <i class="fa-solid fa-dollar"></i>200
                    </div>
                    <p class="increase-percentage">$503(%2)</p>
                </div>

                <div class="trans-history d-flex justify-content-between">
                    <p>22.02.15</p>
                    <p class="fw-bold" id="trans-pair">BTC/USDT</p>
                    <div class="b">
                        <i class="fa-brands fa-bitcoin" ></i><span>0.002</span>
                    </div>
                    <div class="d">
                        <i class="fa-solid fa-dollar"></i>200
                    </div>
                    <p class="increase-percentage">$503(%2)</p>
                </div>

                <div class="trans-history d-flex justify-content-between">
                    <p>22.02.15</p>
                    <p class="fw-bold" id="trans-pair">BTC/USDT</p>
                    <div class="b">
                        <i class="fa-brands fa-bitcoin" ></i><span>0.002</span>
                    </div>
                    <div class="d">
                        <i class="fa-solid fa-dollar"></i>200
                    </div>
                    <p class="increase-percentage">$503(%2)</p>
                </div>

                <div class="trans-history d-flex justify-content-between">
                    <p>22.02.15</p>
                    <p class="fw-bold" id="trans-pair">BTC/USDT</p>
                    <div class="b">
                        <i class="fa-brands fa-bitcoin" ></i><span>0.002</span>
                    </div>
                    <div class="d">
                        <i class="fa-solid fa-dollar"></i>200
                    </div>
                    <p class="increase-percentage">$503(%2)</p>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'DashboardView',
  components: {
    
  },
  data: function() {
      return{
          isSwitched: false
      };
  },
  methods: {
      buy: function() {
          this.isSwitched = false;
      },
      sell: function() {
          this.isSwitched = true;
      }
  }
}
</script>
