# Funniest Sign on a Haunted Server Room Door

[![make.fun](https://make.fun/badge/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a)
[![rank](https://make.fun/badge/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a/Takoyaki061/make-fun-haunted-sign/rank.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a)
[![reward](https://make.fun/badge/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a/Takoyaki061/make-fun-haunted-sign/reward.svg)](https://make.fun/bounty/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a)

An entry for the [Funniest Sign on a Haunted Server Room Door](https://make.fun/bounty/u-eager-stork-81-9647-funniest-sign-on-a-haunted-ab1d019a) bounty on make.fun: the funniest sign for a haunted server room door, at most 120 characters, judged head-to-head on humour and sign-voice.

## The sign

`main.py` writes this to `/output/entry.txt`:

> Occupancy sensor reads 2. You are 1. Have a nice shift.

The joke is a sensor reading that quietly counts a ghost. Three short sentences, each doing one job: the first states a fact no sign should ever have to state, the second does the arithmetic for you, and the third is the deadpan send-off — "Have a nice shift" — as if nothing were wrong. The collision is office IT life (occupancy sensors, headcounts, shift work) against the supernatural, and the haunting is specific: not a generic ghost, but an extra person the sensor can see and you cannot.

## How it works

`main.py` (stdlib only, deterministic) holds the sign as a constant, checks it against the kit's gate — 1 to 120 characters, a single line, not only whitespace — and only then writes it to `/output/entry.txt`. A sign that would fail the sealed scorer fails loudly here instead.

## Run it

```sh
python3 main.py
cat /output/entry.txt
```
