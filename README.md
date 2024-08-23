## Moov_bootcamp Uyo
This is the overview of what I learnt on aleo blockchain using the leo language

# Installation 

I am using Windows Os, so I had to use the Microsoft Visual installer so I could install Rust and use the Cargo cli

then I cloned the Leo programming repo https://github.com/ProvableHQ/leo and switched to the testnet-beta branch

we created three programs and deployed them


![image](https://github.com/user-attachments/assets/c51917fe-3a94-4047-9327-d1542255d57b)

# Workshop 1
The first program was a simple Leo progam that add two variables together and mine was deployed here

`leo run main 3u32 2u32 --network testnet`
Where main =》transition function name, `3u32 2u32` is the inputs and network is specified `testnet`

https://testnet.aleoscan.io/transaction?id=at1emfdahu6nyzjd5djdxtagpf9tfrun8er3v3ysy280xfp5exswuqsfw8ltm


# Workshop 2
The second program was create a token. We used the mint and transfer functions(transitions) then deployed the token to the testnet


1st Command : `leo run mint <type_aleo_address> <type_amount>u64`


2nd command: `leo run transfer "<Token_Record>" <to_address> <amount>u64`
We were  able to use the generated record from 1st command to input into the second command's first input  and then our to address and amount 

 https://testnet.aleoscan.io/transaction?id=at1at0epvkm5f6fsuku9kg49u84gqm9p80dt3dc4q78r9akjt846yqspfkvnw

 # Workshop 3 

`leo run combine_hash_owner_receiver <type_your_address> <type_friend_address>`
This has only 2 inputs where first input is owner address (self.caller) and second input is the  receiver address

https://testnet.aleoscan.io/transaction?id=at1emfdahu6nyzjd5djdxtagpf9tfrun8er3v3ysy280xfp5exswuqsfw8ltm