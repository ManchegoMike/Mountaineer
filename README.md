# Mountaineer

A World of Warcraft addon to support the Hardcore [Mountaineer Challenge](http://tinyurl.com/hc-mountaineers). Designed for Season of Mastery.

Created by ManchegoMike ([Twitch](https://www.twitch.tv/ManchegoMike), [GitHub](https://github.com/ManchegoMike))

This addon is not intended to be "judge and jury" for your Mountaineer Challenge, nor is it the final arbiter of what is or isn't allowed. It doesn't *prevent* you from doing anything; it's simply a way to alert you to some obvious issues and keep you on the straight and narrow.

## Installation

You can do all of these steps *while the game is running*.

* Click the green `Code` button near the top of this page and select `Download ZIP`.
* When the ZIP file has finished downloading, find it on your computer & unzip it into your Interface\AddOns folder.
* The folder you just unzipped will most likely be named `Mountaineer-main`. Rename it to `Mountaineer`.
* Start WoW, or type `/reload` if it's already running.

## Features

* When your brand new level 1 character enters the game for the first time, all your gear is removed and placed into your backpack so you can sell it.

* Each time you login, your gear is checked to make sure you're not wearing anything you shouldn't.

* The primary way the addon determines if gear is allowed is by looking at how you got it. If you got it via looting, then it's fine. If you got it via quest or vendor, then it's only allowed if it's a recipe, a crafting reagent, or a miscellaneous weapon like a skinning knife, mining pick, or fishing pole. Otherwise it's a disallowed item. This is not an infallible method, but it seems to work. Even so, you can override the addon’s determination in case it makes a mistake.

* Whenever you try to equip a disallowed item, you get a warning.

* Whenever you enter combat while wearing a disallowed item, you get a warning.

* Whenever you level up, your skills are checked to make sure you're on track. You'll get a warning if you're falling more than 25 points behind where you should be (your level x 5).

* Whenever you enter a resting area (city or inn), you'll see a message gently reminding you not to logout there.

* If you are a hunter and you cast [Revive Pet](https://classic.wowhead.com/spell=982/revive-pet), you will get a reminder that you need to abandon your pet.

* None of the bonus challenges are supported by the addon at this time.

## Usage

You can use the console command `/mtn` or `/mountaineer`.

All of the following settings are global to your WoW account, so if you turn off sound or allow an item on character A, it will be the same for character B and *all* your characters.

#### `/mtn sound on/off`

Turns addon sounds on or off

#### `/mtn allow {id/name/link}`

Allows you to equip/use an item. You can specify by id# or name or link. Examples: `/mtn allow 7005`, `/mtn allow Skinning Knife`

To specify a link, type `/mtn allow` followed by a space, then SHIFT-click the actual item and it will paste the link into the text you're typing.

#### `/mtn disallow {id/name/link}`

Disallows an item. You can specify by id# or name or link. Examples: `/mtn disallow 7005`, `/mtn disallow Skinning Knife`

To specify a link, type `/mtn disallow` followed by a space, then SHIFT-click the actual item and it will paste the link into the text you're typing.

## Limitations

- U.S. English is the only language supported. If you play in another language, the parsing won't work when you receive a new item.
- Bags are only checked (to see if you're allowed to use them) when you receive them, but not when you equip them.
- If you start using the addon with a character past level 1, it will assume everything you own is approved, unless you saw it previously on some other character and it was disapproved then.

## Wish list

- I'd like to include something in an item's mouse-hover text to indicate whether it's OK to use, but that would make this addon *significantly* more complex.

## Bug reports

Please submit tickets via [GitHub](https://github.com/ManchegoMike/Mountaineer/issues).

## Thanks

Many thanks go to my fellow O.G. Mountaineers:

- [Flipmode31](https://www.twitch.tv/flipmode31), who came up with the initial idea for the Mountaineer Challenge.
- [Briadan](https://www.twitch.tv/briadan), who bravely tested several characters and provided valuable feedback.