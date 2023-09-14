# Patterns-with-javascript-DSA->

1)half diamond pattern ->
*
**
***
****
*****
*****
****
***
**
*


 for(var i=1; i<=5; i++){
            var str = "";

            for(var j=1; j<=i; j++){
                str = str + "*";
            }
            console.log(str);
        }
        // now for reverse star 
        for(var k=1; k<=5;k++){
            var str ="";
            for( var l=5; l>=k; l--){
                str = str+"*";
            }
            console.log(str);
        }

=====================================================================================================================================
2)adjacent triangle star pattern->

*    *
**   **
***  ***
**** ****
**********

        //main loop
       for(var i =1 ; i<= 5; i++){

        //loop to print 1st half
        var str = "" 
        for(var j=1; j<=i ; j++){
            var str = str + "*";
        }
        //loop to print spaces before printing another star
        for (var k=i; k<5; k++){
             str = str + " ";
        }
        //now the last loop to print final triangle 
        for(var l =1; l<=i ; l++){
            str = str +"*"
        }

     console.log(str);
       }

=====================================================================================================================================

3) reverse triangle-> 

*****
****
***
**
*

for (var i=1; i<=5; i++){
    var str = "";
        //second loop starting from 5 going till 1 
    for(var j=5; j>=i; j--){
        str = str + "*";
    }
    console.log(str);
}


=====================================================================================================================================

4) print-> 

*****
****
***
**
*
*
**
***
****
*****

//first loop to print reverse triangle 
        for(var i=1; i<=5; i++){
            var str = ""; 
            //second loop to do the printing inside the first pattern 
            for(var j=5; j>=i; j--){
                str = str + "*";
            } 
            console.log(str)
        }
            // //now we starty third loop to print simple triangle below 
            for(var k=1; k<=5; k++){
                var str = ""
                //4th loop to do the printing inside the straight triangle 
                for( var l=1; l<=k; l++){
                    str = str+"*"
                }
                console.log(str);
            }

=====================================================================================================================================

5) number triangle 

1
12
123
1234
12345

//first loop to print number of lines  
        for( var i=1; i<=5; i++ ){
            var num = " ";
        //second loop iterates and adds the value of i in num starting from 1
            for(var j=1; j<=i; j++){
                num = num + j; 
            }
            console.log(num )
        }


=====================================================================================================================================

6) square pattern 

*****
*****
*****
*****
*****

var str = "";
      //first loop for 5 lines
      for (var i = 0; i < 5; i++) {
        //second loop prints star in each line 
        for (var j = 0; j < 5; j++) {
          str = str + "*";
        }
        str += "\n";
      }
      console.log(str);


=====================================================================================================================================

7) right triangle 

    *
   **
  ***
 ****
*****

 let string = "";
       //outer loop for printing 5 lines
for (let i = 1; i <= 5; i++) {
  // printing spaces
  for (let j = 0; j < 5 - i; j++) {
    string += " ";
  }
  // printing star
  for (let k = 0; k < i; k++) {
    string += "*";
  }
  string += "\n";
}
console.log(string);

=====================================================================================================================================
