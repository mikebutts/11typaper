---
layout: blog-layout.liquid
title: this is the contact page
---

<h3 class="row flex-center margin-bottom-large">Send us a message</h3>
<div class="row flex-center">
<form
  action="https://formspree.io/xvowydar"
  method="POST"
>
  <label>
    Your email:
    <input type="text" name="_replyto">
  </label>
  <label>
    Your message:
    <textarea name="message"></textarea>
  </label>

  <!-- your other form fields go here -->

<button type="submit">Send</button>

</form>
</div>
