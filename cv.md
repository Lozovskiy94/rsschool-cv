# Lozovskiy Bogdan
## Contact information:
1. **Location:** Ukraine, Krivoy Rog
2. **Phone:** +38 096 413 57 51
3. **E-mail:** lozovskiy94@gmail.com
## About Me:
I want to learn Front-End Development in RSSchool!
## Skills:
* HTML (basics)
* CSS (basics)
* JavaScript (basics)
## Code Example:
Build Tower
Build a pyramid-shaped tower, as an array/list of strings, given a positive integer number of floors. A tower block is represented with "*" character.

For example, a tower with 3 floors looks like this:

[
  "  *  ",
  
  " *** ", 
  
  "*****"
]

And a tower with 6 floors looks like this:

[
  "     *     ", 
  
  "    ***    ", 
  
  "   *****   ", 
  
  "  *******  ", 
  
  " ********* ", 
  
  "***********"
  
]
``` 
function towerBuilder(nFloors) {
  // build here
  let arr = []
  let star = '*'
  let a = 1
  let space = ' '
  
  //prepare arr length
  
  for (i = 0; i < nFloors-1; i++) { 
      if (a % 2 == 1)  {
        a = a + 2    
      }
   }
   
  //prepare arr
  
  for (i = 0,j = nFloors - 1; i < nFloors; i++,j--) {
      let start = new RegExp (`^\\*{${j}}`, `g`)
      let end = new RegExp (`\\*{${j}}$`, `g`)
     arr.push(star.repeat(a).replace(end, space.repeat(j)).replace(start,space.repeat(j)))
  }
  //delete spaces in last child
  let lastOne = arr[arr.length-1].trim()
  arr[arr.length-1] = lastOne
  return arr
}
```
## Experience:
## Education:
* **University:** State University of Economics and Technology, Master`s Degree field of study "Mechanical Engineering"
* **Courses:** RS Schools Course «JavaScript/Front-end. Stage 0» (in progress)
## English:
A2 
