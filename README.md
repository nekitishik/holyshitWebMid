# holyshitWebMid
### This is my repository
### My name is @nikkwebdev
![](https://images.saymedia-content.com/.image/t_share/MjAxNzQ2NzkyNTQxMzMzMjY4/biography-adolf-hitler.jpg)

* i am web developer from Tatariv
```javascript

    let url = "https://raw.githubusercontent.com/MamboDancer/WebMiddleCyberween/main/task.json"

function drawlist(link) {
    fetch(link).then(async result => {
        const data = await result.json();
        console.log(data.event)
        document.querySelector('h1').innerHTML = ` 
            <h1>${data.event}</h1>`

        data.guests.forEach(guest => {
            document.querySelector(".guests").innerHTML += `
                <div class="guest">
                    <p class="name">${guest.name}</p>
                    <p class="about">${guest.about}</p>
                    <img src="${guest.photo_url}" alt="${guest.name}">
                </div>
            `
        });

    })
}

drawlist(url)

```

* [president](http://facebook.com/donaldtrump)