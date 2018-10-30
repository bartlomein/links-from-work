# links-from-work

#OVERALL DEV
https://medium.com/datadriveninvestor/stopping-using-console-log-and-start-using-your-browsers-debugger-62bc893d93ff

#REACT
https://vx-demo.now.sh/



#STORYBOOK 
https://www.learnstorybook.com
https://www.sitepoint.com/react-storybook-develop-beautiful-user-interfaces-with-ease/




let arr =[
  {
    title:'test',cam:'live'
  },
  {
     title:'test',cam:'weather'
  },
  {
     title:'test',cam:'live'
  },
  { title:'test',cam:'weather'
  },
  { title:'test',cam:'weather'
  },
  { title:'test',cam:'live'
  },
  { title:'test',cam:'live'
  }
]
let testarr=[];
let newtest = arr;

l = arr.length;
arr[-1] = arr[l-1]; // this is legal
arr[l] = arr[0];

for(i = 0; i < l; i++)
{
    previous = arr[i-1];
    current = arr[i];
    next = arr[i+1];
    
    if(previous.cam !=='weather' || current.cam!=='weather'){
    testarr.push(current)
    }
}

// restore the array
console.log(testarr)
arr.pop(); 
arr[-1] = null;

