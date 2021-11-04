# My thoughts about the JSBooru.

It does a few things exactly how I would expect it to, and how I would have done it if I'd written the code myself.

# Database

## Pros
- Images are collected in a "database"-esque JSON file. Each element in the JSON file contains a URL to the image, a post ID, an array of tags, a rating.
- New tags are confirmed with a prompt, and added to a "tags.json" file. Each tag is also given a unique ID.
- Uploaded images are moved into a dedicated pictures folder.

## Cons
- The file names are scrambled into some random sequence, as well as the IDs. I would have just given each "post" an integer value, starting at 1, and incrementing +1 for each new image. It'd be much simpler, as well as more human readable. Plus it would also have the benefit of giving you a "history" of the order of posts.
- Only one kind of tag -- No support for characters, authors, artists, type, category, collections, etc. Though I imagine it would be easy to implement.
- No bulk uploading -- images have to be added one-at-a-time, and tags manually added for each image.
- Also due to the weird scrambled/random IDs, you can't really do manual bulk adding by just editing the JS files. You'd need to know how to create these IDs in a way that doesn't conflict with the system, which basically locks you in to using the "booru upload" as the only valid method.

# Things I would add
Other than the above stated fixes to the Cons, here's some other features I'd like:

- [ ] File Type Tags on the images (indicators for PNG, GIF, etc)
- [ ] Add a +/- button add/remove tags. Ideally, this would work similar to Calibre.
- [ ] Add a folder for "_unprocessed" which would allow bulk processing of images.
- [ ] Ability to bulk-process through CSV spreadsheet.
- [ ] Ability to export and import the JSON as CSV.
- [ ] Add a proper "index" page that is plain HTML, which I can have links to specific "collections" or tag search queries.
- [ ] "Random" button which just selects a random image. Would be a lot easier with sequential integer IDs.
- [ ] Filter for NSFW and SAFE (there seems to be a tag for it, but you can't filter by it)
- [ ] Ability to attach a "comment" or "note" to an image post. This would just be some simple plain text, I would imagine. That way I can record some of my original thoughts when finding an image.
- [ ] Expand the note function later to be able to link MarkDown posts to Images.
- [ ] Also, support for MarkDown posts, in general.

# Closing Notes
Check out Gelbooru.com for inspiration on layout and formatting.

This looks pretty straightforward. I should be able to modify this pretty easily to my needs.

# Some inspiration, things to add to the Booru
- [mogeko (okegom), alice (alice in wonderland), funamusea, oounabara to wadanohara, 1girl, alice (alice in wonderland) (cosplay), apron, bangs, biscuit (bread), black eyes, black footwear, black ribbon, blue dress, blush, braid, brown hair, bunny, candy, card, coffee, coffee cup, coffee mug, cosplay, cup, disposable cup, dress, food, full body, hair ribbon, heart, key, lollipop, long hair, looking to the side, mug, mushroom, open mouth, red background, ribbon, shoes, short sleeves, simple background, skirt, sugar cube, teapot, twin braids, white apron, white background, white skirt - Image View - | Gelbooru - Free Anime and Hentai Gallery](https://gelbooru.com/index.php?page=post&s=view&id=6481158&tags=open_mouth) - Cute Alice in Wonderland

- [mouri kazuaki, alpha (dream hunter rem), ayanokouji rem, beta (dream hunter rem), dream hunter rem, 1980s (style), official art, scan, 1girl, bag, blue eyes, bread, capelet, cat, dog, food, green hair, grocery bag, holding, holding bag, long hair, long sleeves, looking at viewer, mary janes, open mouth, red footwear, red skirt, retro artstyle, shoes, shopping bag, skirt, walking - Image View - | Gelbooru - Free Anime and Hentai Gallery](https://gelbooru.com/index.php?page=post&s=view&id=5457076) - I want to learn how to do this 80's watercolor style.

- [mouri kazuaki, ayanokouji rem, dream hunter rem, 1980s (style), highres, official art, 1girl, bangs, barefoot, bra, full body, green hair, long hair, measuring, oldschool, panties, retro artstyle, simple background, solo, tape measure, underwear, underwear only, white background, yellow bra, yellow panties - Image View - | Gelbooru - Free Anime and Hentai Gallery](https://gelbooru.com/index.php?page=post&s=view&id=6480926) - I want to learn how to do this 80's watercolor style.

