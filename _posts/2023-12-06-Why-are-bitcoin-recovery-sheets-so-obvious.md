---
published: true
---

This is something that I was thinking about recently.

I get that brands want to slap their logo on whatever, but who is going to be sharing a picture of their recovery sheet?

Maybe it is so you don’t confuse it with your other sheets of 24 words that you have stored?

Whatever the reason, considering how important this list of words is, I don’t think you should be giving any clues on what they mean. 

<img src="/images/novel" width="50%" alt="Recovery Sheet">

## The idea behind the Novel Wallet

For the past few years, my job has revolved around digital assets like Bitcoin, meaning, the importance of security has been beaten into my head.

I don’t believe that a single paper wallet should be the sole method of custody, but rather a mixture and geographic distribution of the many options (hardware, multisig, metal, etc) out there.

The idea of the [Novel Wallet](https://novelwallet.com) did not come from a place of maximum security, but rather, just an idea I thought was cool.

I’ve always enjoyed stories about finding lost treasure and I do think in the future, there will instances of people recovering lost wallets from odd places and this somewhat played into the thinking behind the Novel Wallet.

Why make it is easy for your grandkids to access to your hoard of Bitcoin?

Give them a mysterious book, with some personalized note written on the first page riddled with clues to a potential fortune.

Ok, obviously that is not the purpose and you should really consider a succession plan or telling someone you trust how to access your funds in case you get hit by a bus.

But, my thinking was that it is easy to lose a piece of paper, but mistakenly throwing out a hardcover book takes more effort.

I then thought about how to hide the BIP39 words in the book.

Sure, you could just take any book off your shelf and write your seed phrase in it however you please.

But, I thought it would be cool if you had a story that incorporated the words seamlessly, so as not to seem out of place.

To manage expectations, Novel Wallet is not an eloquent story of BIP39 words, but rather a prototype that has every BIP39 word appearing once in every chapter.

## What is BIP39?

BIP39 stands for "Bitcoin Improvement Proposal 39." It's a standard introduced to improve the way we handle and secure our cryptocurrency wallets. Originating from the Bitcoin community, it's now widely used in many other cryptocurrencies as well.

So, why was BIP39 introduced? 

Before this, managing and restoring crypto wallets was a bit of a headache. If you lost access to your wallet, it was pretty much game over for your digital coins.

BIP39 changed the game by introducing mnemonic phrases—a set of 12 to 24 random words derived from a list of 2048 designated words.

These words effectively act as a backup for your wallet.

## How does the Novel wallet work?

It’s pretty simple.

There are 24 chapters in the book and, in each chapter, every BIP39 word will appear once.

Let’s say the eleventh word of your seed phrase was “jaguar” you would go through chapter eleven, find the word “jaguar” and highlight it or put some marking that you would recognize and then move onto chapter twelve to find the next word of your seed phrase.
In the end you would have 24 words highlighted or marked in some way within the book and that’s it.

<img src="/images/jaguar" width="50%" alt="How Novel wallet works">


## Creating the Novel Wallet

This proved to be a lot harder than expected.

Let’s break this down into 3 parts:

### 1. Novel contents

This was the easiest part, I found a public domain book (bonus points if you can guess the book after it has had the BIP39 words merged in), that conveniently had 24 chapters.

Since there are 2048 words within the BIP39 wordlist, I tried to make sure that every chapter had at least 5000 words, this involved some copy and pasting, but overall, it wasn’t that difficult of a task.

### 2. Randomly inserting words into the novel

This and the next part were outsourced because I am not a developer.

It seemed that putting the words into the document via script was not too hard. 

Adding some thresholds so that the words that were being replaced were of similar length helped the structure of the book appear somewhat normal from first glance.

### 3. Mapping those words to their pages

This is where it got tricky. It seemed that page numbers on word could not be read via Python script, so the document had to first replace the words, then convert to PDF then map the page numbers that way.

This is still not perfect and page numbers are more of “it might be on this page or the previous”.

## I am open sourcing this for individual use

You can find the script that I used on [Github](https://github.com/boomahora/NovelWallet).

Here is the [print PDF](https://github.com/boomahora/NovelWallet/blob/main/Novel%20Wallet%20-%20Full%20content.pdf) so that you can print it yourself if you want maximum anonymity.

You can also buy the [prototype](https://www.amazon.com/dp/B0CN3YGBHM) from Amazon if you don’t want to go through the hassle of printing.

Here is the [list of BIP39 words mapped](https://github.com/boomahora/NovelWallet/blob/main/Word%20page%20locations.xlsx) to their possible page numbers.

## Quick disclaimer here

Your seed phrase is super important, so please take all the precautions necessary. 

I really believe that you can’t be too safe when it comes to your seed phrase.

## Why did I make this?

Simply because I thought it would be a fun weekend project (although it took a bit longer than a weekend).

It’s not a million-dollar idea and will not change the world, but it was fun to do.

If you want to follow my next weekend project feel free to connect with me on [Linkedin](https://linkedin.com/in/alexthecannon) or you can follow my [newsletter](https://alexcannon.substack.com/). 
