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
    
    //my first smart contract in solidity web 3.0 
   
    
    // SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract Counter {
    uint public count;

    // Function to get the current count
    function get() public view returns (uint) {
        return count;
    }

    // Function to increment count by 1
    function inc() public {
        count += 1;
    }

    // Function to decrement count by 1
    function dec() public {
        // This function will fail if count = 0
        count -= 1;
    }
}

 //my first smart contract in solidity web 3.0 
   
    
    // SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract Counter {
    uint public count;

    // Function to get the current count
    function get() public view returns (uint) {
        return count;
    }
    
    <h2>My First JavaScript</h2>

<button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>

<p id="demo"></p>

</body>
</html> 

// Numbers:
let length = 16;
let weight = 7.5;

// Strings:
let color = "Yellow";
let lastName = "Johnson";

// Booleans
let x = true;
let y = false;

// Object:
const person = {firstName:"John", lastName:"Doe"};

// Array object:
const cars = ["Saab", "Volvo", "BMW"];

// Date object:
const date = new Date("2022-03-25");
let x = "Volvo" + 16 + 4;
let x = 16 + 4 + "Volvo";
