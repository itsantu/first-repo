## First-repo
Hey its my first repo
<br>
And I'm gonna continue the series
```javascript
const a = "Antu";
console.log("My name is ", a); 
```

# API REQUEST

```javascript
const requestUrl = 'https://api.github.com/users/hiteshchoudhary'
const xhr = new XMLHttpRequest()
xhr.open('GET', requestUrl)
xhr.onreadystatechange = function(){
    console.log(xhr.readyState)
    if (xhr.readyState === 4){
        const data = JSON.parse(this.responseText)
        console.log(data.followers)
    }
}
xhr.send()
```