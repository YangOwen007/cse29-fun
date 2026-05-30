# My Animation Page

<style>
.fade-in {
  opacity: 0;
  animation: fadeIn 2s ease-in forwards;
  font-size: 32px;
  color: dodgerblue;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<div class="fade-in">
  Hello! This text fades in.
</div>
