---
layout: page
title: contact
permalink: /contact/
description: You can contact me by filling out the form below or by shooting me a message on LinkedIn.
nav: true
nav_order: 1000

social: true
---

<form id="fs-frm" name="simple-contact-form" accept-charset="utf-8" action="https://formspree.io/f/mrgnpddd" method="post">
    <fieldset id="fs-frm-inputs">
        <div class="mb-3">
            <label for="full-name" class="form-label">Full Name</label>
            <input class="form-control" type="text" name="name" id="full-name" placeholder="First and Last" required>            
        </div>
        <div class="mb-3">  
            <label class="form-label" for="email-address">Email Address</label>
            <input class="form-control" type="email" name="_replyto" id="email-address" placeholder="email@domain.tld" required>
        </div>
        <div class="mb-3">
            <label class="form-label" for="message">Message</label>
            <textarea class="form-control" rows="5" name="message" id="message" placeholder="Type your message here." required></textarea>                   
        </div>
        <input type="hidden" name="_subject" id="email-subject" value="Contact Form Submission">        
    </fieldset>
    <button type="submit" class="btn btn-primary">Submit</button>
</form>

<br>
<!-- Social -->
{% if page.social %}
<div class="social">
    <div class="contact-icons">{% include social.liquid %}</div>
</div>
{% endif %}
