# Final_Assessment_Module3_ETH

This is the Solidity software, commonly known as the minting and burning software; it will show you how to mint and burn the token, as well as the total supply of the token.

## Description

For MetaCrafters' final assessment, I created an ethereum token that will mint, burn, and know the overall supply of the token.


## Getting Started



### Executing program

* To begin with look remix.etheruem.org at that point once you open the site discover the make a unused record at that point named it like this (name).sol at that point put the code at that point put your title on token title and to the token abbrevation. once you wrap up the code, Tap the robustness compiler then compile your record. on the off chance that you're wrap up compiling the code you'll presently press the send and run exchanges at that point duplicate the account and utilize it the address of the burning,minting and equalizations once you wrap up putting the account of the address at that point input a esteem at that point execute to begin with execute the stamping to store the token at that point to burn the token fair press the execute button on the burning. And on the off chance that you mint 3 token at that point you burn 4 nothing will happen since you surpass the store esteem of the mint.
```
//SPDX-License-Identifier: MIT
        pragma solidity ^0.8.18;


        contract metacrafters{

                     // public variables here
                string public TokenName = "Anime Token";
                string public TokenAbbrv = "ATT";
                uint public TotalSupply = 0;

                       // mapping variable here 
                 mapping (address => uint) public Balances; 

                      // minting variable here
                  function Minting (address Address, uint Value)public{
                            TotalSupply += Value;
                            Balances [Address] += Value;
                    }
                      
                      // burning variable here
                  function Burning (address Address, uint Value)public{
                           if(Balances[Address] >= Value){
                            TotalSupply -= Value;
                            Balances [Address] -= Value;}
                   } 

        } 
```

## Help

Simply examine the code for missing symbols like,, (,), [], and ;. Please always check for errors per line. If there is an issue, your file name will change red, or a red symbol will appear on the left side of the number, indicating that there is an error.

```
(), {}, [], ;

```

## Authors

Aristhotel R. Arroyo
8213426@ntc.edu.ph

## License

This project is licensed under the [MIT] License - see the LICENSE.md file for details
