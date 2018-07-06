# No.4 Product Gallery

---

## [DEMO](dist/)

## [spec](https://hexschool.github.io/THE_F2E_Design/week4-product%20gallery/)

## Note

### animation(baber-pole, 霓虹燈效果) for repeating-linear-gradient

- [CSS repeating-linear-gradient() Function](https://www.w3schools.com/cssref/func_repeating-linear-gradient.asp)
- [CSS Repeating Gradients](https://css-tricks.com/snippets/css/css-repeating-gradients/)
- [A Striped Barberpole Animation](https://css-tricks.com/books/volume-i/striped-barberpole-animation/)

```css
.pattern {
  background-image: repeating-linear-gradient(
    135deg,
    $color-blue,
    $color-blue 18px,
    transparent 10px,
    transparent 34.5px
  );
  /* 必須設 size 才能有移動效果 */
  background-size: 200% 200%;
}

@keyframes barber-pole {
  100% {
    background-position: 100% 100%;
  }
}

.pattern:hover {
  animation: barber-pole 10s linear infinite;
}
```
