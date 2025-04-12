# TODOstr

TODOstr is a public TODO board where anyone can post TODOs or zap TODOs posted by others. It's completely vibe-coded. Nostr relays enable the app to run without its own backend.

Created using VSCode + Roo Code plugin (Google Gemini 2.5 pro). The initial working prototype was made in 3 prompts (initial + 2 follow-ups). I did not add or edit any of the code in index.html. The AI wrote everything.
I've continued refining the app. Go to the original prototype repository for the first 3 prompts:
[TODOstr original](https://github.com/rolznz/todostr-original)

Try it now: [TODOstr](https://rolznz.github.io/todostr/)

This was inspired by [Max](https://nostrudel.ninja/#/u/npub18lzls4f6h46n43revlzvg6x06z8geww7uudhncfdttdtypduqnfsagugm3)'s [note](https://nostrudel.ninja/#/n/nevent1qvzqqqqqqypzq079lp2n40t48tz8je7yc35vl5yw3juaaecm08sj6kk6kgzmcpxnqyfhwumn8ghj7ur4wfcxcetsv9njuetn9uq3zamnwvaz7tmwdaehgu3wwa5kuef0qqsz9l6hk0dwa6f9lww7qts93p4upnletesnc4t23y7ug08glyzpjdc8tgtal)

> I'm going to a hackathon this Saturday and I'd like to showcase to a new community the power of nostr and lightning zaps. I have 2 ideas that I would like to prototype (I'm currently vibe coding them but unlikely I'll have them totally ironed out before then). I will pay a bounty of100,000 sats each via zap (so a total of 200k sats up for grabs) for a live working web version + code/prompts for each of these ideas.

One of the ideas was:

> A meme generator with nostr login and zaps. You include 5 or so popular meme templates (guy looking at girl, winnie the pooh, etc) and allow anyone to enter their own text. They're then able to share theire memes via popular nostr relays and other users are able to zap their favorite memes. A leaderboard shows the most popular memes by global zaps and by the zaps of your follows. (I'm also open to using other WoT calcs but I assume that's too complex.) You should be able to login via a browser extension like alby, paste a priv key, or spin up a new nostr identity.

However, I think it's too difficult currently for 1-shotting YET so I will pull out some more complicated parts of the original query. I've changed it to be a zappable TODO list which still ecompasses some of the core nostr features.

```txt
A TODO list with nostr login and zaps. You allow anyone to enter their own TODOs. They're then able to share them via popular nostr relays and other users are able to zap their favorite TODO items. A leaderboard shows the most popular TODO items by global zaps. You should be able to login via a browser extension like alby.
```

Follow-ups:

1. Deleting a TODO
2. A leaderboard shows the most popular TODO items by global zaps and by the zaps of your follows. (I'm also open to using other WoT calcs but I assume that's too complex.)
3. You should be able to login via a browser extension like alby, paste a priv key, or spin up a new nostr identity
4. Allowing uploading images to nostr.build and attaching them in the TODO item.

Notes: for Alby to work you need to serve the index.html file. I ran `python3 -m http.server` in the same directory for this.

See my follow-up prompts in follow-ups, each is put in a separate commit.