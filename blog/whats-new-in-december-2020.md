# What's new in December 2020?

Hello everyone! 

We were thinking it would be a good idea to regularly share with you some of the new things we've done during the month so you can feel part of our little community!

If we get a positive response we might even make this a regular thing.

Let us know in our telegram group or by hitting that smiley face at the bottom of the article. :\)

## New Netflix Regions!

Thanks to L for recommending us some IP ranges that work with Netflix, we are now able to unblock Netherlands, Turkey, and Russia Netflix. 

This brings our total supported regions to 14.

These regions were added on the 6th of December.

## Updated Routing For NETFLIX and \[CHINA\] Servers

Before, the NETFLIX servers had a special routing. Users from outside China would connect to the servers directly, whereas users from with China would be redirected to a \[CHINA\] server for better speeds.

However, this caused some stability issues for users within China because after being connected to a foreign server for the some time, the v2ray app itself would start to think that they were actually in another country and would then redirect them to the slower, direct connection instead.

This switch back and forth between routing would cause disconnections and instability.

Therefore, we are now discontinuing this special routing.

**NETFLIX servers will now connect directly even for users in China.**

We will add these servers to the \[CHINA\] list instead.

If you are in China, please use the \[CHINA\] NETFLIX servers and NOT the NETFLIX servers for the best speeds.

This change will provide better stability, plus simplify our work on the back end. Less things will go wrong on a simpler setup. 

## Redesigned Dashboard

We've redesigned our entire client area to make it easier to navigate.

#### The main dashboard

On the main dashboard, you can now quickly access download files, APIs, and links to our setup guides for 12 different apps. 

Below that, you'll find the section for managing your subscription, with the renewal date and a 'renew' button as well as a collapsible menu for changing your API codes, purchasing a new subscription, and cancelling your current subscription.

A similar dashboard is available for each VIP subscription.

#### Extend subscription button

The "extend subscription" button can now be used to renew your membership ahead of time.

If an invoice does not exist, you will be redirected to a page where you can select the legnth of time you want to renew your subscription for. 

If an invoice already exists, you will be redirected to pay for that invoice instead so no duplicate invoices are created.

#### SmartDNS page removed

We've removed the SmartDNS page in favor of an easily-accessible box on the main dashboard. You can now easily update your IP and select your prefered Netflix region directly from the front page.

#### Eclipse

In the same spirit, we've updated the Eclipse page with a similar look and feel.

#### Invoices page

The invoices page now no longer show unpaid invoices that are over 1 month past due. This prevents clutter.

If you want to renew your subscription and it has ran out for over 1 month, please purchase a new subscription instead or renewing your old one.

#### Services page

This page is now accessible from the main dashboard, by clicking on the "Active services" button.

The services page no longer shows subscriptions that have run out or have not been paid for over a month. 

If you want to renew your subscription and it has ran out for over 1 month, please purchase a new subscription instead or renewing your old one.

## New Chatbot

You may have noticed a new chatbot once you login. This is a chat bot. Not a live human. We have programed it to answer the most common questions and to do basic troubleshooting.

{% hint style="info" %}
Please do not expect an immediate answer from a live human by typing into the chat box. It is a robot. Please open a support ticket or send us a message on telegram instead.
{% endhint %}

#### How the chatbot works

You will be presented with a list of options to choose from. The chat bot can resolve about 70% of issues.

This means that you have a good chance of fixing your problem immediately by using the chat bot before opening a ticket.

Why not try it out the next time your have an issue? :\)

## New Servers

### New US Server

We are happy to announce our 18th city in our network, New York! 

New York is fast for those accessing US content from Europe or the Middle East, so we've added New York as our first east-coast server.

### Additional servers for popular regions

We added an additional server cluster to our Hong Kong, Los Angeles, Japan, and Germany locations to provide redundancy and to expand our network capacity for our most popular regions.

## New Locations Page

We now have a "locations" page that shows where our servers are and which ones unblock Netflix.

You can have a look [here](https://wannaflix.com/locations.php).



