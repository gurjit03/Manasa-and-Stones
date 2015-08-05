 function processData(input) {
   
    function getCombinations(emptySpaces,a,b) {
        
       var combinations = '';
        
        if(!(a === b)){
            if(a < b) {
                 var aLoop = emptySpaces - 1, bLoop = 0;        
                 // Ascending Loop
                while(!(aLoop < 0)) {

                    var firstStone = 0;
                    firstStone += aLoop * a;
                    firstStone += bLoop * b;
                   --aLoop; 
                   ++bLoop;
                  combinations += firstStone + ' ';
                  }
            }
            else {
                //desceding loop
                var aLoop = 0, bLoop = emptySpaces - 1;        
                 // Ascending Loop
                while(!(bLoop < 0)) {

                    var firstStone = 0;
                    firstStone += aLoop * a;
                    firstStone += bLoop * b;
                   --bLoop; 
                   ++aLoop;
                  combinations += firstStone + ' ';
                  }
            }
            console.log(combinations);
            } else {
                var aLoop = emptySpaces - 1, bLoop = 0; 
                
                var firstStone = 0;
                firstStone += aLoop * a;
                firstStone += bLoop * b;
                console.log(firstStone);
            }
        }
    
    
    //Enter your code here
    var inputArray = input.split('\n');
    var T = Number(inputArray[0]);
    var counter = 1;
    
    while(T--) {
         getCombinations(Number(inputArray[counter]),
                                  Number(inputArray[counter + 1]),
                                  Number(inputArray[counter + 2]));
        counter += 3;
    }
    
} 

process.stdin.resume();
process.stdin.setEncoding("ascii");
_input = "";
process.stdin.on("data", function (input) {
    _input += input;
});

process.stdin.on("end", function () {
   processData(_input);
});
