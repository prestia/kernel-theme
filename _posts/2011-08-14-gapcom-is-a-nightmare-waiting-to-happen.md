---
layout: post
category : writings
tags : [security, ecommerce, gap, banana republic, old navy, piperlime, athleta]
title: Gap.com is a Nightmare Waiting to Happen
---
{% include JB/setup %}

I discovered today that the entire family of Gap websites (gap.com, bananarepublic.com, oldnavy.com, piperlime.com, and athleta.com) store customer passwords in plain text. This is particularly worrisome because these websites also store the customer's name, address, email, phone number, and credit card number. It is possible that the credit card numbers are properly hashed (I have no way to verify), but this still wouldn't prevent massive fraud if someone were to steal the customer database and post it online.

If you shop at any of these websites and have your personal data stored, now would be a great time to delete it.