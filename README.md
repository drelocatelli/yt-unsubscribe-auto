# Youtube unsubscribe auto

1. [Entre nesse link](https://www.youtube.com/feed/channels)

2. Cole esse código no console do navegador:
```
function desinscrever(){
    document.querySelectorAll("#subscribe-button > ytd-subscribe-button-renderer > paper-button").forEach(function(unsubscribeBtn){

    setTimeout(function(){ unsubscribeBtn.click()}, 3000)
    setTimeout(function(){ document.querySelector("#confirm-button > a").click() }, 3000)
    window.scrollTo(0,document.body.scrollHeight);

    })
    
}
desinscrever()
```
