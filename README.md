# acc_test

## 1. Describe yourself
####   My name is Girijapathi Math, from Karnataka India. I like to play badminton and listen to music to keep positive intent. Completed Masters in Computer Applications from Bangalore university in 2014. Professionally I have total of 4.6 years experience, from past 3 years  working as we web developer.

## 2. You discover a bug in the codebase. What steps do you take?
#### 1. Gather codebase version information, log files if any, error message/bug details if not provided. 
#### 2. Try to re-create the bug at in-house setup.
#### 3. Once issue could re-create at in-house/ develooper accessible test/dev environment, going through stack trace of issue and figure out which face of code introduced bug and possible solutions.
#### 4. Coding the best possible solution and demoing to team and if there is better solution adopt it and provide fix.
#### 5. Making development team about the scenario which introduced bug.



## 3. Describe the kinds of tests you would write at various points in the SDLC
#### 1. Unit testing and Graybox testing  the code during development.
#### 2. Integration testing after completing the development phase.

## 4.
```javascript
describe("ZIP Code Formatter ", => {
    it("validate if input string is not empty", () => {

    });
    describe("standard ZIP ", () =>{
        it("returns formatted ZIP for valid length string",() =>{});
        it("adds leading zero if input string length is less than five and returns formatted ZIP",() =>{});
    });
    describe("standard+4 format of ZIP ", () => {
        it("returns formatted string for ten character length string",() =>{});
        it("validates if input string has minimum length of 6",() =>{});
        it("appends zeros if string length is less than 10",() =>{});
    });
});
```

## 5.
#### DNS: Stands for Domain Name System. It is a protocol/rule different parties adhere to exhange data over internet through TCP/IP protocol. When a URL is requested browser contacts DNS to get respective IP address. For example if URL www.google.com is requested form browser, DNS would return 12.34.456.78. In simple terms DNS is look up place to get IP address for given URL. Best example would be Phone's address book, I would store Home contact number as 1234-567, so when I want to call no need to dial number just click on Home, then mobile would look for  number respective to Home and dial.


## 6.
```javascript
function calculateSum(coins, target) {
    var result = []; 
    if(coins == null || coins.length == 0) return result;
 
    var current = [];
    coins.sort();
 
    findCombination(coins, target, 0, current, result);
    // return best combination
    return result[result.length-1];
}
 
function findCombination(coins, target, j, curr, result){
   if(target === 0){
       var temp = curr.slice();
       result.push(temp);
       return;
   }
 
   for(var i=j; i<coins.length; i++){
       if(target < coins[i]) 
            return;
       curr.push(coins[i]);
       findCombination(coins, target - coins[i], i, curr, result);
       curr.pop(); 
   }
}
```


