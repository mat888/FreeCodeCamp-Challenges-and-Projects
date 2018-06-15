function whatIsInAName(collection, source) {
 
  var arr = [];
  
  for (var i = 0; i < collection.length; i++) {
  
    var n = 0;

    loop0:
    for (var j = 0; j < Object.keys(source).length; j++) {
      //console.log(Object.keys(source).length);
      //console.log(collection[i][Object.keys(source)[j]]);
      //console.log(Object.values(source)[j]);
      
      if (collection[i].hasOwnProperty(Object.keys(source)[j]) && collection[i][Object.keys(source)[j]] == Object.values(source)[j]  ) {
        
        console.log('aa');
        //console.log(Object.values(source)[j]);
        
        for(var k = 0; k < Object.keys(collection[i]).length; k++) {
          
          //console.log(Object.keys(collection[i]));
          //console.log(Object.keys(source));
          //console.log(Object.keys(source).includes(Object.keys(collection[i])[1]));
          
          if (Object.keys(source).includes(Object.keys(collection[i])[k])) {
            console.log('bb');
            n += 1;
            //console.log(k);
            }
          
          }
        
        if (n == (Object.keys(source)).length){
          console.log(i);
          console.log(j);
          console.log(k);
          console.log('sec if');
          console.log(collection[i]);
          arr.push(collection[i]);
          
          break loop0;
        }
          
        
      }
      
    }
  
  
  }
  //arr.push(collection[0]);
  console.log('end');
  console.log(arr);
  return arr;
}

    console.log(whatIsInAName(whatIsInAName([{ first: "Romeo", last: "Montague" }, { first: "Mercutio", last: null }, { first: "Tybalt", last: "Capulet" }], { last: "Capulet" })));
