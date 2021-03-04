## Gleb Pissarik 

### Contacts
* 4ebula@gmail.com
* +375 29 230 86 80
* https://t.me/Chebula
* [github](https://github.com/4ebula)

---

### About me

My goal is to change career and become a front end developer. Have a passion for codding.
I'm very attracted to the opportunity to learn creating mobile apps and SPA.
Great learner; like to discover new approaches and ways, always strive to improve myself. Can easily find elegant and efficient solutions to non-standart tasks.

---

### Skills

Have basic knowledge in HTML5, CSS3, JS and C++, experience with Bootstrap and jQuery, Git Version control.
Background in supporting site with CMS (Joomla).
English level is somewhere about B1.

---

### Education  

Self-educated.

---

### Code example

```javascript
function timerStarter(){
  minutes = +currentTime[0];
  seconds = +currentTime[1];
 setTimeout(function tick(){
    if(isStarted && minutes+seconds != 0 && !isReset) {
      if(firstStart) {
        seconds++;
        firstStart = false;
      }
      circleProgress();
      countdown();
      setTimeout(tick, 1000);
      if(minutes+seconds == 0){
        isReset = true;
        let counter = false;
        let colorNow;
        let bgRing = document.getElementsByClassName('backgroundCircle')[0];
        let time = document.getElementById('clockLength');
        setTimeout(function blink(){
          sound.play();
          colorNow = counter & 1 ? '#fe4e4d' : '#0dc97f';
          time.style.color = colorNow;
          bgRing.style.setProperty('stroke', colorNow);
          counter = !counter;
          if(isReset == false) {
            sound.pause();
            document.getElementsByClassName('backgroundCircle')[0].style.setProperty('stroke', '#9ca5b5');
            time.style.color = '#fe4e4d';
            return;}
          setTimeout(blink, 550);
        }, 0);
        isReset = true;
        
        timer();
      }
    }
  }, 0);
}
```