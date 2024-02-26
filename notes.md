
https://github.com/dark0rder/wise-lending-codebase-code4rena/blob/a25334e72e74f7539f0bcdc0234af88c438affcf/contracts/WiseLending.sol#L255-L269

https://github.com/dark0rder/wise-lending-codebase-code4rena/blob/gurvinder/contracts/WiseLendingDeclaration.sol#L322-L326

https://github.com/dark0rder/wise-lending-codebase-code4rena/blob/gurvinder/contracts/WiseLendingDeclaration.sol#L299-L302

## (--Doubts--not sure--)

Function _getCurrentSharePriceMax might return inaacurrate APR , which might lead to other bugs, inaccuracy in APY AND APR for borrowers and lenders.

  // APR RESTRICTIONS
    uint256 internal constant RESTRICTION_FACTOR = 10
        * PRECISION_FACTOR_E36
        / PRECISION_FACTOR_YEAR;
}

 uint256 internal constant PRECISION_FACTOR_YEAR = PRECISION_FACTOR_E18 * ONE_YEAR;
 
 uint256 internal constant ONE_YEAR = 365 days;



## All about Leap Years:
A leap year is a year with 366 days instead of the usual 365. This additional day is added to February, making it 29 days long instead of 28. Leap years occur approximately every four years
