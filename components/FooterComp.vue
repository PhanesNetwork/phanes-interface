<template>
    <footer class="row footer">
         <div class="h-line"></div>
      <div class="columns">
          <div class="col1">
              <img src="@/assets/logo.png" alt="" class="logo">
              <div class="social-icons">
                  <a href="https://twitter.com/phanes_network" target="_blank"><img src="~/assets/Twitter.png" alt=""></a>
                  <a href=""><img src="~/assets/discord.png" alt=""></a>
                  <a href="https://t.me/phanes_anns" target="_blank"><img src="~/assets/telegram.png" alt=""></a> 
                  <a href="https://t.me/phanes_anns"target="_blank"><img src="~/assets/announcement.png" alt=""></a> 
              </div>

          </div>

          <div class="col">
            <h3 class="title">Products</h3>
            <ul class="items">
                <li class="item"><a href="https://app.phanes.network" target="_blank">Staking Vault</a></li>
                <li class="item"><a href="https://app.phanes.network/" target="_blank">Phanes Wallet</a></li>
                <!--
                <li class="item"><a href="https://phanes.network/multisender" target="_blank">Multisender</a></li>
                <li class="item"><a href="https://phanes.network/minter" target="_blank">Minter</a></li> -->
                
            </ul>
        </div>
          
         <div class="col">
            <h3 class="title">Important Links</h3>
            <ul class="items">
                <li class="item"><a href="https://docs.phanes.network/phanes-tokenomics/phanes-token" target="_blank">Governance</a></li>
                <li class="item"><a href="https://docs.phanes.network/products/phanes-index-portfolio" target="_blank">Indices</a></li>
                <li class="item"><a href="https://docs.phanes.network/" target="_blank">Documentation</a></li>
                
            </ul>
        </div>
          <div class="col">
              <h3 class="title">Support</h3>
              <ul class="items">
                <li class="item"><a href="https://contact@phanes.network" target="_blank">Contact</a></li>
                <li class="item"><a href="https://blog.phanes.network" target="_blank">Blog</a></li>
               
              </ul>
          </div>
      </div>
      <div class="h-line"></div>
      <div class="copyright-text">
          <p class="text">Copyright © 2022 Phanes Network</p>
          <div class="right-links">
              <span>All Rights Reserved </span>|
              <a href="https://docs.phanes.network/conclusion/disclaimer" target="_blank"> Terms and Conditions </a>|
              <a href="" target="_blank"> Privacy Policy</a>
          </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style lang="scss" scoped>
      .footer{
          padding-bottom: 50px;
          .columns{
              padding: 109px 24px;
              display: flex;
              align-items: flex-start;
              justify-content: space-between;
              @media only screen and (max-width:720px){
                  display: grid;                
                  grid-template-columns: repeat(1,1fr);
                  grid-gap: 20px;
                  padding:  60px 24px;
              }
              .col1{
                  .logo{
                      height: 60px;
                      margin-bottom: 38px;
                      @media only screen and (max-width: 580px){
                          height: 40px;
                          margin-bottom: 20px;
                      }
                  }
                  .social-icons{
                      display: flex;
                      align-items: center;
                      &>*:not(:last-child){
                          margin-right: 24px;
                          @media only screen and (max-width: 580px){
                            margin-right: 15px;
                          }
                      }
                      a{
                          img{
                              width:24px;
                              height: 24px;
                              @media only screen and (max-width: 580px){
                                width: 18px;
                                height: 18px;
                              }
                          }
                      }
                  }
              }
              .col{
                  .title{
                      font-weight: 700;
                      font-size: 20px;
                      line-height: 22px;
                      color: #1BD19C;
                      margin-bottom: 40px;
                      @media only screen and (max-width:720px){
                          margin-bottom: 20px;
                      }
                      @media only screen and (max-width: 580px){
                          font-size: 18px;
                          line-height: 20px;
                      }
                  }
                  .items{
                      list-style: none;
                      .item a{
                          text-decoration: none;
                          font-weight: 400;
                          font-size: 18px;
                          line-height: 20px;
                          color: #EDEDED;
                          transition: all .2s;
                          @media only screen and (max-width: 580px){
                              font-size: 15px;
                              line-height: 15px;
                          }
                          &:hover{
                              color:#FFFFFF;
                              font-size: 20px;
                          }
                          
                      }
                      .item{
                          margin-bottom: 18px;
                          @media only screen and (max-width: 580px){
                              margin-bottom: 10px;
                          }
                      }
                  }
              }
          }
          .h-line{
              width: 100%;
              height: 0px;
              border: 1px solid #4f558086;
              margin-bottom: 25px;
          }
          .copyright-text{
              display: flex;
              align-items: center;
              justify-content: space-between;
              font-weight: 400;
              font-size: 18px;
              line-height: 30px;
              color: #EDEDED;
              @media only screen and (max-width:580px){
                  font-size: 14px;
                  line-height: 18px;
              }
              @media only screen and (max-width:920px){
                  flex-direction: column;
                  justify-content: center;
              }
  
              .right-links{
                  @media only screen and (max-width:580px){
                      font-size: 12px;
                      line-height: 18px;
                  }
                  @media only screen and (max-width:380px){
                      font-size: 8px;
                  }
                  a{
                      text-decoration: underline;
                      color: #1BD19C;
                  }
              }
          }
      }
  </style>
