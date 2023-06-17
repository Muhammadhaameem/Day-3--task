# Day-3--task
question no.1

let obj1=
{"name":"person1","age":5}
let obj2=
{"age":5,"name":person1}
console.log(obj1==obj2)


question no.2
var request=new XMLHttpRequest()
    request.open('GET','https://restcountries.com/v3.1/all')
    request.send()
    request.onload=function()
    {
        var data=JSON.parse(request.response)
        console.log(data[0])
        for(var i=0;i<data.length;i++)
        {
console.log(data[i].flags)
        }
    }


    question no. 3
    
 var request=new XMLHttpRequest()
    request.open('GET','https://restcountries.com/v3.1/all')
    request.send()
    request.onload=function()
    {
        var data=JSON.parse(request.response)
        console.log(data[0])
        for(var i=0;i<data.length;i++)
        {
console.log("country name - " +data[i].name.common+"; region - "+data[i].region+"; sub region - "+data[i].subregion+"; population - "+data[i].population)
        }
        }
