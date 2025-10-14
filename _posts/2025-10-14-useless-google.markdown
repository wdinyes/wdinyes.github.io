---
layout: post
title:  "Google's Security Is Shit"
date:   2025-10-14 05:00:00 -0700
categories: general
---

A little background: my iPhone got run over repeatedly last week, and I then needed to set up a new one, without a lot of access to some items, particularly OTP codes stored in Google Authenticator.

Now, in the past, I have used Google Authenticator quite successfully, and when moving between phones, was able to simply migrate the data and have all of my precious OTP codes pop up without issue.  But not this time.

Why?  Because in April of 2023, Google introduced [cloud syncing of the 2FA codes](https://techcrunch.com/2023/04/24/google-authenticator-can-now-sync-2fa-codes-to-the-cloud/).  I had been using this tool for long enough that I didn't even really notice it getting updated.  It may have prompted me for an account to use, but I can't recall clearly.

In any event, I updated my phone that year without any issues.  I suspect local storage was probably still in use, and the data migration happened in the usual way.

This time around, though, I found two things amiss: First, Authenticator had, somehow, stopped allowing the local storage to migrate.  And second, it had associated all my codes with my work Google Account, rather than my personal Google Account.

Now, this is important, because I had been trying to keep my work and personal accounts separated on my iPhone.  It seems Google had other plans, looked at how I was using my accounts (work gets more interaction than personal, at least on my work phone - Drive, Sheets, Docs, Google Mail and Calendar, all those Google apps use my work account, with my personal account using more of the iOS equivalents), and decided to associate my 2FA codes with my work account.  The problem being, it created a catch-22 for me when I tried to recover the account on my new phone.  If my 2FA codes are stored with my work account, and I cannot get into my work account without the 2FA code, I'm royally fucked.

I did eventually manage to get around it with some clever hacks like taking screenshots of QR codes, and then uploading those to my iMac (yes, I tried iPhone mirroring, no, it didn't work - the damage was too extensive, an antenna was damaged, the camera module on the phone was non-functional, just a mess).  The screen was largely illegible, but I could get enough information out of it to know when a QR code was displayed.

In any event, I spent the next couple of days divesting myself of anything in Google Authenticator, and made updates to some of my Google Accounts, including updating an old password on an older account that had an alert about being in a data breach.

And here's where the second part of Google's bullshit kicks in.

Google lets you set up 2FA and passkeys on your accounts.  Now, call me crazy if you like, but if I have a passkey and 2FA and a password, Google should be pretty well aware that it's me trying to do whatever it is I'm trying to do.  I updated the old account to have all three, integrated with Apple's Passwords tool (because seriously, fuck Google forever now).  The latest version allows you to store passkeys and even generates OTP 2FA codes.  This is fantastic (not unique, 1Password can also do this, and I presume most other tools can as well - I'm telling you this because you need to dump Google Authenticator, seriously, what a joke), and means I have a very clear way to prove I am who I say I am.

Or so I thought.

I can log in to the old account on the webpage, I can get my emails, all that is fine.  But when I opened my iOS mail app, I was told I needed to re-enter the password on the old account.  Since it's the one I had just updated, this seemed reasonable.

Ha!

So, I open the account settings, click to enter my password, and am presented with the browser-based login to the Google account.  Fine!  It even gives me the option to use my passkey!  Amazing, I think, this is so much simpler.

Provide passkey.  Get message . . .

"Google couldn't verify this account belongs to you."

Um, bitch, it's my passkey.  The one I *just* created a couple hours ago.  

Oh, I can try to recover my account.  Sure, OK, go through those steps, enter password this time, enter 2FA key, both of which I had confirmed as working through Safari.

"Google couldn't verify this account belongs to you."

The fuck?  OK, once more, this time using one of my 8 digit recovery keys, the ones that I am ***LOOKING AT RIGHT NOW ON ANOTHER BROWSER WINDOW USING THE SAME CREDENTIALS I AM TRYING TO USE TO LOG IN TO MY FUCKING EMAIL***, and what do I get?

"Google couldn't verify this account belongs to you."

Oh my God, ***FUUUUUUUUUUCK*** you, Google.

What is the goddamn problem?  There's no indicator.  All I can find online is that maybe it's because I'm logging in from an unknown location.  Like that should even fucking matter, ***WHEN I HAVE A GODDAMN PASSKEY!!!!!***

Maybe there's a trigger of too many attempts.  Fine!  Let me go into my account another way and fucking tell you it's me!  Nope.  There's security warnings that some attempt or another was blocked, but clicking on "Yes, it was me," does absolutely fucking nothing.

I'm sure Google's answer is, "Just use the GMail app."

No, assholes, that's for work, and I deliberately never open that app on the weekends or after hours.  I'm not putting my personal goddamn email in there, and I certainly don't want to risk replying to a work email with a personal email address.

The real answer is, Google security is shit.  Utter fucking shit.  They have no qualms about locking me out of my account for ***LITERALLY*** no fucking reason, but I hear all the time about accounts getting hacked and scammed and lost to malicious actors.

I.  Have.  A.  Pass.  Key.  It cannot be accessed without biometric confirmation from me.  It's mine.  It proves it's me.  That's what the fucking things were designed for!  You, yourselves, claimed it was a more secure method of authentication than using 2FA and passwords, you even fucking encouraged all of us to use them!  And now?

"Google couldn't verify this account belongs to you."

Eat a dick, Google.  Eat a huge bag of rotting zombie dicks.
