# My Animation Page

<link rel="stylesheet" href="style.css">

<div class="fade-in">
  Hello! This text fades in.
</div>

# Scroll Animation Example

Scroll down to see the animation.

Here is some extra text to make the page longer. This helps us test scroll animations because the page needs enough space to scroll.

Here is another paragraph of filler text. Later, this could be replaced with real information about your website, your project, or the animations you are testing.

Here is one more paragraph before the first scroll animation. Keep scrolling down to see the animated text appear.

<div class="scroll-fade">
  This text fades in when you scroll to it.
</div>

Here is more filler text after the first animation. The goal is to create enough space so that the next animation starts off-screen.

This paragraph is here so you can scroll away from the first animation and then scroll back to replay it.

<div class="scroll-fade">
  This one also replays when you scroll back to it.
</div>

<script>
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.remove("animate");

      // Forces the animation to restart
      void entry.target.offsetWidth;

      entry.target.classList.add("animate");
    } else {
      entry.target.classList.remove("animate");
    }
  });
});

document.querySelectorAll(".scroll-fade").forEach(element => {
  observer.observe(element);
});
</script>
