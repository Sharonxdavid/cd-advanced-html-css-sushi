## ವಿಶೇಷ ಪರಿಣಾಮಗಳು

ಈ ಕಾರ್ಡ್‌ನಲ್ಲಿ ನೀವು ಸಿಎಸ್‌ಎಸ್‌ನೊಂದಿಗೆ ಸಾಧಿಸಬಹುದಾದ ಇನ್ನೂ ಕೆಲವು ಉತ್ತಮ ಪರಿಣಾಮಗಳನ್ನು ಕಲಿಯುವಿರಿ.

### ನೆರಳುಗಳು ಮತ್ತು ಚಲನೆ

ನೀವು ಮೊದಲು ಮಾಡಿದ ಕಾರ್ಡ್‌ಗಳ ಮೇಲೆ ನಿಮ್ಮcursor ಅನ್ನು ಸುಳಿದಾಡಿದಾಗ ಸ್ವಲ್ಪ ಚಲನೆಯನ್ನು ಸೇರಿಸೋಣ.

+ `.card:hover` ಅನ್ನು ಹುಡುಕಿ ಮೊದಲಿನಿಂದ ಸಿಎಸ್ಎಸ್ ವರ್ಗ ಮತ್ತು ಅದನ್ನು ಈ ಕೆಳಗಿನವುಗಳಿಗೆ ಬದಲಾಯಿಸಿ:

```css
    .card:hover {
        box-shadow: 0px 2px 2px rgba(0,0,0,0.2); 
        transform: translateY(-2px);
    }
```

+ `translate` function ವಿಭಿನ್ನ ಮೌಲ್ಯಗಳನ್ನು ಪ್ರಯತ್ನಿಸಿ!

--- collapse ---
---
title: transform ಆಸ್ತಿ
---

ನೀವು ಮಧ್ಯಂತರ HTML / CSS ಸುಶಿ ಕಾರ್ಡ್‌ಗಳನ್ನು ಪೂರ್ಣಗೊಳಿಸಿದರೆ, `transform` ರವನ್ನು ನೀವು ನೆನಪಿರಬಹುದು ಕೆಲವು `@keyframes` ನಲ್ಲಿನ ಆಸ್ತಿ ಅನಿಮೇಷನ್. ಸಾಮಾನ್ಯ ಸಿಎಸ್ಎಸ್ ಬ್ಲಾಕ್ನಲ್ಲಿ ನೀವು ಆಸ್ತಿಯನ್ನು ಸ್ವಂತವಾಗಿ ಬಳಸಬಹುದು ಎಂದು ಇಲ್ಲಿ ನೀವು ನೋಡುತ್ತೀರಿ.

ನೀವು ಅದನ್ನು ಹೊಂದಿಸಬಹುದಾದ ಒಂದು ರೀತಿಯ ಮೌಲ್ಯ `rotate`, ಒಂದು ಅಂಶ ತಿರುವು ಮಾಡಲು. ಇತರರು `translateY`, ಅದು ಏನನ್ನಾದರೂ ಮೇಲಕ್ಕೆ ಅಥವಾ ಕೆಳಕ್ಕೆ ಚಲಿಸುತ್ತದೆ ಮತ್ತು `translateX`, ಅಕ್ಕಪಕ್ಕಕ್ಕೆ ಚಲನೆಗಾಗಿ.

--- /collapse ---

+ `box-shadow`ಗಳಲ್ಲಿ ವಿಭಿನ್ನ ಪಿಕ್ಸೆಲ್ ಮೌಲ್ಯಗಳೊಂದಿಗೆ ಆಟವಾಡಿ ಅವರು ಏನು ಮಾಡುತ್ತಾರೆಂದು ನೋಡಲು ಆಸ್ತಿ. 

--- collapse ---
---
title: ಏನು `rgba`?
---

`rgba (0,0,0,0.2)` ಬಣ್ಣವನ್ನು ವ್ಯಾಖ್ಯಾನಿಸುವ ಇನ್ನೊಂದು ವಿಧಾನ.

ಇದು ಸಾಮಾನ್ಯ ಮೂರು ಸಂಖ್ಯೆಗಳನ್ನು ಪಡೆದುಕೊಂಡಿದೆ (`0` ರಿಂದ `255` ವರೆಗೆ) ಕೆಂಪು, ಹಸಿರು ಮತ್ತು ನೀಲಿ ಬಣ್ಣಗಳಿಗೆ.

ನಾಲ್ಕನೇ ಸಂಖ್ಯೆ, ಇದನ್ನು **alpha** ಎಂದು ಕರೆಯಲಾಗುತ್ತದೆ ಮೌಲ್ಯ, ಹೇಗೆ **transparent** ಎಂದು ವ್ಯಾಖ್ಯಾನಿಸುತ್ತದೆ (ಅಥವಾ ನೋಡಿ-ಮೂಲಕ) ಏನೋ. ಇದು `0` ನಡುವಿನ ದಶಮಾಂಶ ಸಂಖ್ಯೆ ಮತ್ತು `1`, `1` ರೊಂದಿಗೆ ಎಲ್ಲವನ್ನು ನೋಡುವುದಿಲ್ಲ, ಮತ್ತು `0` ಸಂಪೂರ್ಣವಾಗಿ ಅಗೋಚರವಾಗಿರುವುದು. ಇದರರ್ಥ ಒಂದು ಅಂಶದ ಆಲ್ಫಾ ಮೌಲ್ಯ ಕಡಿಮೆ, ಅದನ್ನು ಹೆಚ್ಚು ನೋಡುವ ಮೂಲಕ.

--- /collapse ---

+ ಅಂತಿಮವಾಗಿ, ಈ ಕೆಳಗಿನ ಆಸ್ತಿಯನ್ನು `.card` ‌ಗೆ ಸೇರಿಸುವ ಮೂಲಕ ಚಲನೆಯನ್ನು ಸುಗಮಗೊಳಿಸಿ ಮೊದಲಿನಿಂದ ವರ್ಗ: 

```css
    transition: all 0.2s ease-out;
```

`0.2s` ನ ಅವಧಿ ಎಂದರೆ `transition` 0.2 ಸೆಕೆಂಡುಗಳವರೆಗೆ ಇರುತ್ತದೆ.

### ಲೈಟ್‌ಬಾಕ್ಸ್

ಬಹಳಷ್ಟು ವೆಬ್‌ಸೈಟ್‌ಗಳಲ್ಲಿ ನೀವು ಬಹುಶಃ ನೋಡಿದ ಮತ್ತೊಂದು ಪರಿಣಾಮವೆಂದರೆ **lightbox**: ನೀವು ಯಾವುದನ್ನಾದರೂ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ವೆಬ್‌ಸೈಟ್ ಮಂಕಾಗುತ್ತದೆ, ಆದರೆ ದೊಡ್ಡ ಚಿತ್ರ ಅಥವಾ ಪಾಪ್ಅಪ್ ಬಾಕ್ಸ್‌ನಂತೆ ಬೇರೆ ಯಾವುದಾದರೂ ವಿಷಯದ ಮುಂದೆ ಕಾಣಿಸಿಕೊಳ್ಳುತ್ತದೆ.

![ಕ್ರಿಯೆಯಲ್ಲಿ ಲೈಟ್‌ಬಾಕ್ಸ್ ಪರಿಣಾಮ](images/lightboxLemur.png)

ಈ ಪರಿಣಾಮವನ್ನು ಪಡೆಯಲು ನೀವು ಎರಡು ಲಿಂಕ್‌ಗಳನ್ನು ಮಾಡುತ್ತೀರಿ: ಒಂದು ನಿಜವಾದ ಲೈಟ್‌ಬಾಕ್ಸ್‌ಗೆ (ಪಾಪ್ ಅಪ್ ಆಗುವ ಬಿಟ್), ಮತ್ತು ಲೈಟ್‌ಬಾಕ್ಸ್ ಗೋಚರಿಸಲು ನೀವು ಕ್ಲಿಕ್ ಮಾಡಿದ ವಿಷಯಕ್ಕೆ ಒಂದು. ನನ್ನ ವೆಬ್‌ಸೈಟ್‌ನ ಆಕರ್ಷಣೆಗಳ ಪುಟದಲ್ಲಿ ನಾನು ಗಣಿ ಮಾಡಲು ಹೋಗುತ್ತೇನೆ. ನೀವು ಚಿತ್ರಗಳನ್ನು ಹೊಂದಿರುವ ಯಾವುದೇ ಪುಟದೊಂದಿಗೆ ನೀವು ಹೋಗುತ್ತೀರಿ!

+ ನೀವು ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ನೀವು ಯಾವ ವಿಷಯಗಳನ್ನು ಕಾಣಿಸಿಕೊಳ್ಳಲು ಬಯಸುತ್ತೀರಿ ಎಂಬುದನ್ನು ನಿರ್ಧರಿಸಿ, ಮತ್ತು `a` ಗುಂಪಿನ ನಡುವೆ ಎಲ್ಲವನ್ನೂ ನಿಮ್ಮ ಪುಟಕ್ಕೆ ಸೇರಿಸಿ ಲಿಂಕ್ ಮಾಡಲು ಟ್ಯಾಗ್‌ಗಳು. ನೀವು ಲಿಂಕ್‌ಗೆ `id` ನೀಡಿದ್ದೀರಿ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ. ಕೋಡ್ ಪುಟದಲ್ಲಿ ಎಲ್ಲಿಯಾದರೂ ಹೋಗಬಹುದು: next step ನಲ್ಲಿ ನೀವು ಅಂಶಗಳನ್ನು ಅಗೋಚರವಾಗಿ ಮಾಡುತ್ತೀರಿ!

```html
    <a href="#_" class="lightbox" id="boxLemur">
        <h3>Lemur!!</h3>
        <img src="monkey-2223271_640.jpg" alt="Picture of a lemur" />
        <p>A lemur enjoying a little snack</p>
    </a>
```

ಲಿಂಕ್ ಟ್ಯಾಗ್‌ಗಳ ನಡುವೆ ನೀವು ಇಷ್ಟಪಡುವದನ್ನು ಹಾಕಬಹುದು. ನನಗೆ ದೊಡ್ಡ ಚಿತ್ರ, ಶೀರ್ಷಿಕೆ ಮತ್ತು ಕೆಲವು ಪಠ್ಯ ಸಿಕ್ಕಿದೆ. ಬಹುಶಃ ನೀವು ಚಿತ್ರವನ್ನು ಬಯಸುತ್ತೀರಿ ಮತ್ತು ಪಠ್ಯವಿಲ್ಲ!

+ ಲೈಟ್‌ಬಾಕ್ಸ್‌ಗಾಗಿ ಈ ಕೆಳಗಿನ CSS ಕೋಡ್ ಸೇರಿಸಿ. ಅದರಲ್ಲಿ ಕೆಲವು ಏನು ಮಾಡುತ್ತದೆ ಎಂದು ನೀವು ಕೆಲಸ ಮಾಡಬಹುದೇ?

```css
    .lightbox{
        background: rgba(0,0,0,0.8);
        color: #ffffff;
        text-align: center;
        text-decoration: none;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        position: fixed;
        visibility: hidden;
        z-index: 999;
    }
```

ಗಮನಿಸಿ: `position` ವನ್ನು ಹೊಂದಿಸಲಾಗುತ್ತಿದೆ ಆಸ್ತಿಯನ್ನು `fixed` ಇದರರ್ಥ ನೀವು ಹೊಂದಿಸಿದ ಸ್ಥಾನವು browser windowಗೆ ಸಂಬಂಧಿಸಿರುತ್ತದೆ, ಆದ್ದರಿಂದ ನೀವು ಸ್ಕ್ರಾಲ್ ಮಾಡುವಾಗ ಅದು ಉಳಿಯುತ್ತದೆ.

+ ಮುಂದೆ, ಲೈಟ್‌ಬಾಕ್ಸ್ ಗೋಚರಿಸಲು ನೀವು ಯಾವ ವಿಷಯವನ್ನು click ಮಾಡಬೇಕೆಂದು ನಿರ್ಧರಿಸಿ, ಮತ್ತು `a` ಜೋಡಿಯನ್ನು ಸೇರಿಸಿ ಆ ಅಂಶದ ಸುತ್ತಲೂ ಟ್ಯಾಗ್‌ಗಳು (ನನ್ನ ವಿಷಯದಲ್ಲಿ ಇದು ಲೆಮೂರ್‌ನ ಸಣ್ಣ ಚಿತ್ರ). **target** ಲಿಂಕ್‌ನ ಲೈಟ್‌ಬಾಕ್ಸ್ ಆಗಿರುತ್ತದೆ, ಅದನ್ನು ನೀವು `id` ಬಳಸಿ ಹೊಂದಿಸುತ್ತೀರಿ. ಮೊದಲಿನಿಂದಲೂ ನೀವು ಈ ತಂತ್ರವನ್ನು ಗುರುತಿಸಬಹುದು!

```html
    <a href="#boxLemur">
        <img src="monkey-2223271_640.jpg" class="mediumPics">
    </a>
```

+ ಅಂತಿಮವಾಗಿ ಕೆಳಗಿನ CSS ಕೋಡ್ ಸೇರಿಸಿ. ಇದು **pseudo-class** ಎಂಬುದನ್ನು ಗಮನಿಸಿ; ಅದು `.lightbox` ವರ್ಗದ ಕೋಡ್‌ನ ನಂತರ ಹೋಗಬೇಕು ಮತ್ತು ಅದರ ಒಳಗೆ ಇರಬಾರದು!

```css
    .lightbox:target {
        visibility: visible;
    }
```

`:target` ಕೊನೆಯ ಲಿಂಕ್ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಲೈಟ್‌ಬಾಕ್ಸ್ ಗುರಿಯಾಗಿದ್ದಾಗಲೆಲ್ಲಾ ಹುಸಿ ವರ್ಗ ಅನ್ವಯವಾಗುತ್ತದೆ. ಆದ್ದರಿಂದ ನೀವು ಎಲ್ಲಿಯಾದರೂ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ, `visibility` `hidden`.

+ ಲೈಟ್‌ಬಾಕ್ಸ್ ಕಾಣಿಸಿಕೊಳ್ಳಲು ನಿಮ್ಮ ಹೊಸ ಲಿಂಕ್ ಕ್ಲಿಕ್ ಮಾಡಲು ಪ್ರಯತ್ನಿಸಿ! ಅದನ್ನು ಹೋಗಲಾಡಿಸಲು, ಪುಟದಲ್ಲಿ ಎಲ್ಲಿಯಾದರೂ ಕ್ಲಿಕ್ ಮಾಡಿ.

ನೀವು ಪುಟಕ್ಕೆ ಬಯಸುವಷ್ಟು ಲೈಟ್‌ಬಾಕ್ಸ್‌ಗಳನ್ನು ಸೇರಿಸಬಹುದು. ಅವರೆಲ್ಲರೂ ಒಂದೇ CSS ವರ್ಗವನ್ನು ಬಳಸಬಹುದು - ಪ್ರತಿಯೊಬ್ಬರಿಗೂ ವಿಭಿನ್ನ `id` ಇದೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ! ಪ್ರತಿಯೊಂದಕ್ಕೂ, ನಿಮ್ಮwebpageನಲ್ಲಿ ನೀವು ಲೈಟ್‌ಬಾಕ್ಸ್ ಗೋಚರಿಸುವಂತೆ ಕ್ಲಿಕ್ ಮಾಡುವ ಲಿಂಕ್ ಆಗಿ ಏನನ್ನಾದರೂ ಮಾಡಬೇಕಾಗಿದೆ, ತದನಂತರ `id` ಬಳಸಿ `href` ಆಗಿ ನೀವು ಮೇಲೆ ಮಾಡಿದಂತೆಯೇ ಆ ಲಿಂಕ್‌ನಲ್ಲಿನ ಮೌಲ್ಯ!