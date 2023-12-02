# Flow-Beginner-Module3


This Repo is made for an Assessments for the eth-avax Intermediate project for Metacrafters. The purpose of this Repository is to showcase my knowledge and understanding of the smart contracts and especially, about creating my own Tokens,with mentioned requirements.

Description
This Repository consists of a contract named function.sol written in Cadence, a programming language used for developing smart contracts on the Flow blockchain. 

## Getting Started
### Executing program
To run this program, you can use Flow Playboard at https://play.flow.com/


```cadence

 pub contract Product
 pub var infos : { Int  : Info }

pub struct Info {
pub let p_id : Int
pub let p_name: String
pub let p_price : Int
pub let p_quant : Int 


init( _p_id : Int  , _p_name : String , _p_price : Int ,_p_quant : Int)
{
self.p_id = _p_id
self.p_name = _p_name
self.p_price = _p_price
self.p_quant = _p_quant
}
}

pub fun addinfo( p_id : Int , p_name : String , p_price : Int ,p_quant : Int )
{
let newinfo = Info(_p_id : p_id, _p_name : p_name  , _p_price : p_price ,_p_quant : p_quant)
self.infos[p_id] = newinfo
}

init(){
self.infos = { }
}
}
```


To deploy the code, We will be using the Flow Playground

Once the contract is deployed, you can execute the ProductTransaction file provising the appropriate signer and filling the required values.
Onece transaction file is executed , You can execute the ProductScript file to read the function declared in the cadence ProductContract file.

## Authors
Infintecoder100 ((https://github.com/InfiniteCoder100) )

## License
This project is licensed under the MIT- see the LICENSE.md file for details
