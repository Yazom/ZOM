# zom.health
zom.health SmartContracts 
==========================
Clone contract of SushiSwap erc20 Token

- Token Name: zom.health
- Token Symbol: ZOM
- No Max Supply
- Decimal - 18
- Token Contract Name : ZOMHealth

Staking Contract: 
================
Clone Stake contract of SushiSwap MasterChef Stake Contract

- Stake contract name: ZOM_Obsidian
- Reward per block: 2.5 ZOMs
- Reward Duration 1 month ~ 20k blocks
- Bonus multiplier: 5 (i.e initial bonus blocks will distribute 12.5 ZOM per block)
- reward distribution: 85% to the liquidity stakers & 15% to team / dev address.
- Burn Transfer: 
5% per transaction

# Constructor argument during deployment of ZOMCHEF contract:

< zomtoken address >,< dev address >,< 2.5 token with 18 zeros i.e 25 and 17 zeros after it >, < start block >, < bonus end block i.e plus 20k start block >

Note: 10k is for 2 weeks , so if you want 1 month then have to add 20k blocks
      
      check latest block and add 20k to it to be used in contructor arguments

example: "0xFE07E0B64Abe9b4F2AAc8A55b54ccCf08Bf89C6B","0x5A462DA24E01C8edEddD156c35F62318f73b71e6","2500000000000000000","21175773","21195773"

# Adding a pool:

"< allocfactor >","< pool address >",< true >

"100","0x6dd927415800150397cf8868668ba31fd3716481",true

Note: depending on the distribution division you have to decide allocation factor

if LP-A will get twice bonus and LP-B will get single bonus 

LP-A - 200

LP-B - 100

# Changeownership of Token to chef contract:

in the changeownership function of TOKEN CONTRACT, specify the chef address and delegate the ownership to chef contract

# LP Pairs for ZOM.Health

ETH-ZOM - after uniswap listing the address will be available.

UNI-ETH - 0xd3d2e2692501a5c9ca623199d38826e513033a17 (Uniswap mainnet address)

USDT-ETH - 0x0d4a11d5eeaac28ec3f61d100daf4d40471f1852 (Uniswap mainnet address)

USDC-ETH - 0xb4e16d0168e52d35cacd2c6185b44281ec28c9dc (Uniswap mainnet address)

TUSD-ETH - 0xb4d0d9df2738abe81b87b66c80851292492d1404 (Uniswap mainnet address)

DAI-ETH - 0xa478c2975ab1ea89e8196811f51a7b7ade33eb11 (Uniswap mainnet address)



