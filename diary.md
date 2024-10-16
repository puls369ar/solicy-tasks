## [27.09.2024]
* [21:22] - Often new contracts are created with this style `IUniswapV2Pair(pair).initialize(token0, token1);` reminds me of InstanceFactory OOP pattern.


## [28.09.2024]
* [17:15] - Finished learning `UniswapV2Factory` main functionality. New solidity
style is involved, still other features to learn in the contract

## [29.09.2024]
* [19:30] - I realized that I can’t learn common Uniswap functionality in 2 days if I try to interpret each function’s code line by line.
So I divide learning into two levels of complexity, and study the context in a parallel way in order
    L2: Descriptively understand what does the function for the system, what are the inputs and outputs (priority)
    L1: Open the blackbox. Research how code(usually repetitive) works inside functions

* [20:42] - It was a bad idea to explain learned functionality in the code
  with comments. Better migrate them to the `.md` files and collect everything alltogether in git repo.

## [29.09.2024][23:32]
Finished high L2 level research of UniswapV2Router02
Back to finalizing UniswapV2Pait now

## [30.09.2024][14։50]
Viewing the code in road, in smartphone.
Perfect environment(sarcasm)

Why those interfaces and libraries are repetitively defined
in both contracts, sin't there a way to import 
them from predownloaded libraries? Or maybe it is me
that sees only post-macro version of imported
assets.

## [15.10.2024]
* [10:30] - Back to work. Now Learning `Fountain` contract's code and lif3 ecosystem
* [13:00] - Finished learning **ShareWrapper** core contract and **AccessControl**, **ReentrancyGuard** mechanisms everything that is inherited by **Fountain**. Now proceeding to Fountain itself
* [16:00] - Has done half of learning `Fountain` and got a new info about main task. It turns out when we fork `UniswapV2Pair` contract where the swappable oracle is (LIF3(POL),LSHARE(POL)) and deploy it into **lif3** ecosystem where
  **LIF3 coin** is native, it is forbidden or error prone there to have (__LIF3(LIF3)__, LSHARE(LIF3)). I now start to research `Oracle` contract in ModernTreasury
* [19:00] - Today I saw Oracle concept is present in ModernTreasury contract, but needed to finish Fountain contract learning to make everything clear. I finished learning code structure of Fountain contract, check the docs. Will proceed to ModernTreasury tomorrow and after will clarify the logics of both and beautify the contents

## [16.10.2024]
* [18:20] - Finished `ModernTreasury` code revision and docs creation. Generalized some concepts and started creating my own local version of contracts to create better unmessed version of it and write tests on it to understand it better. Will continue to review newly found `Oracle` contract tomorrow.
* [18:50] - The whole structure and the code is in a mess, I'll fix it

## [17.10.2024]
* [11:50] - Got Fountain ecosystem compiled locally!!! changed the version to 0.8.20 and achieved code compatibility
* [16:01] - Got clear compilation with versions for `ModernMasonry` and `ModernTreasury`, but I struggle to get clean results for `Oracle` and it's parent `Epoch`. Some issues with math functions and constructor
  Will give a little pause and continue to clarify the logics of **Fountain**
* [19:02] - Finished Oracle code review and working principle research

## [18.10.2024]
* [14:16] - The decision was made about modifying `BitMath` to work under newer version of solidity that Fountain works with.
  I found [DiffCheck](https://www.diffchecker.com/), great tool to not only observe differences between two files, but also to export it in PDF format. Later I'll collect the differences of original and forked versions of popular smart contracts used in our projects and   keep this PDFs in corresponding folders
* [17:00] - Got the project compiled!!! 

