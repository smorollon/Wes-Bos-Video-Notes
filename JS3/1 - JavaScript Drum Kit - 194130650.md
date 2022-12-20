# JavaScript Drum Kit

A different approach for removing the 'playing' CSS class could be:

```
    window.addEventListener('keyup', function (e) {
      const key = document.querySelector(`.key[data-key="${e.keyCode}"]`);
      if (!key) return;
      key.classList.remove('playing')
    })
```
