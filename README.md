# ETHProject

This starts the basic of utilizing solidity assessment, which is producing a token between all of the modules that have been combined into one.

## Description

This is a unique software that certifies as something evolutionary for decades to come, and it will be able to assist us in navigating the Ethereum blockchain. And in the most conventional way possible; through the realm of code! This demonstrates that blockchain is a stepping stone beyond the horizon.

## Getting started
 ### Executing program
   This is the quickest and most efficient method to learn about Blockchain. Simply navigate to https://remix.ethereum.org/. Then begin with simply tap the addition (+) button and you're ready to code! 
   
```javascript

MyToken.sol

   ```

## 1st Code

    The second step you'd need to copy and paste the code for the final evaluation and then follow Chris' directions on how to combine the remix and coding together effectively.

```javascript
contract MyToken {

    // public variables here
    string public tokenName = "CUTIE";
    string public tokenAbbrv = "CT";
    uint public totalSupply = 0;




```

You will need to enter variables of your Token name and the Abbreviation of that token being a public domain which will assist you distinguish the Name and the Abbreviations.

then begin by mapping the variable using Address => uint as public balances. 
uint is an unsigned int that does not support negative values and also does not add anything, resulting in a zero (0) value for the public variables specified in the code.

## 2nd Code


```javascript

    // mapping variable here
    mapping(address => uint) public balances;

```
It's typically a good idea to make mapping variables public so that everyone may access them. This will pass the mapping area, and because every address begins with an u end, it will provide it to the address, who will return the token amount that the address possesses.

## 3rd Code

You must enter an address and a value that corresponds to the function that raises the overall supply by that number and increases the balance of the address by that amount in the mint section. Because it includes a parameter, it should have an address and a value. I put underscore address and underscore value to distinguish the parameters from the regular values.

```javascript

 // mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances [_address] += _value;
     }
```
In the second, we would need to do the burn and minting operations, which are essentially the same except for the use of '+=' functions on the mint function. In the mint function, the total supply will be raised by the amount of that has already been passed by utilizing the total supply, balances, and the address will be increased by the balances along with the value. 



```javascript
    // burn function
    function burn (address _address, uint _value) public {
        if (balances [_address ] >= _value) {

        totalSupply -= _value;
        balances [_address] -= _value;
        }
        
    }

}

```

The burn function is the inverse of the mint function in that it destroys tokens and eliminates the complete supply and balance from the address entirely. Copy and paste the same function, but execute it in the reverse direction by using the subtraction sign while the plus symbol is beneath it, and you have now received the burn function. You'll be utilizing the inverse, '-='.

Finally, when the burn function is called, you must create a condition to ensure that the balance of the money you received is larger than or equal to the amount that is meant to be burnt and referring to the total supply and the balances together

When you've linked everything, open the "solidity compiler" on the left side of remix.etherium.org and utilize the 'compile my token.sol' button. Once it is completed, it will appear at the bottom of the website with the words "it ran." 


## Running the Code


In addition, click the deploy and run tab, which is found underneath the solidity compiler button. When it opens, you'll notice an orange button labeled deploy, which allows you to check whether your token is available or not. You must first test the waters, i.e. the tokens within the 'deployed contracts'.

Finally, and most crucially, you must copy your account that is pointed towards the depoly, perform transactions, copy paste it, and open the mint and burn below the deployed contracts. Putting them value and copying the account numbers you just acquired into the address form, as well as giving value to the value section. When run by the token abbrv, it will return the amount you just performed. And verifying it with the totalsupply section and the token abbrv, and it's done.


   ### Guide
   Advice and guidance can ask @ the discord with faith/Chris

   ### Author
   Umpar, Aina A.
   @AinaUmpar#1732 on discord
