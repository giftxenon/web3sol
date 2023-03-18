# web3sol
pragma solidity ^0.8.8; // this the version of solidity I choose to use and all versions above it.

contract SimpleStorage {
   
   uint256 public favoriteNumber;
 

   struct People {
       uint256 favoriteNumber;
       string name;
   }
People[] public people;

   function store (uint256 _favoriteNumber) public{

   favoriteNumber = _favoriteNumber;
       }

       function retrieve() public view returns(uint256) {
           return favoriteNumber;

       }
       function addPerson(string memory _name, uint256 _favoriteNumber) public{

           People memory newPerson = People({favoriteNumber: _favoriteNumber, name: _name});
           people.push(newPerson);
       }
    }
