# NameChangeSmartContract: Exploring require(), assert(), and revert()

## Function and Errors

This smart contract demonstrates the usage of `require()`, `assert()`, and `revert()` statements for error handling and ensuring proper contract behavior.

## Description

This Solidity smart contract provides an example of how to use require(), assert(), and revert() to:

* Validate user input during name changes.
* Maintain internal consistency within the contract.
* Prevent unexpected errors.

## Functions and Errors

The contract includes three functions that showcase the use of the mentioned statements:

* changeName(string memory _newName): This function allows users to change their names. It ensures the new name is not empty using require(). Additionally, it limits the number of name changes to three (nameChangeCount) using require(). If either condition fails, the transaction is reverted with a clear error message.
* assertNameLength(): This function is called after a successful name change. It uses assert() to verify the name variable is not empty. If the assertion fails, the transaction is reverted with a generic error message, indicating a potential bug in the logic.
* (Optional, depending on your preference) revertExample(): You could include an additional function (revertExample()) to demonstrate manual revert() usage. For example, it could restrict a specific user address from changing their name.

## Understanding the Statements

* require(): Enforces conditions during function execution. If the condition fails, the transaction is reverted with a custom error message, providing valuable feedback for users and developers.
* assert(): Verifies internal assumptions within the code that should always hold true. If the assertion fails, the transaction is reverted with a generic error message, indicating a potential bug in the code logic.
* revert(): Allows manual transaction reversal with a custom error message. It offers flexibility for tailored error handling within a function (optional in this example).

## License

MIT License

## Author/s

* Danz Andrew M. Permejo (61903256@ntc.edu.ph)

## Getting Started 

This section would typically explain how to deploy the contract to a blockchain network and interact with its functions, but it might not be necessary for a purely educational contract like this one.  


## Help 

This section could provide guidance on troubleshooting common issues or using the contract effectively. 

  
